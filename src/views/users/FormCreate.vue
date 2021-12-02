<template>
    <div>
        <layout-main>
            <div class="d-flex justify-content-between flex-wrap flex-md-nowrap align-items-center pt-3 pb-2 mb-3 border-bottom">
                <h1 class="h2">Create new user</h1>
            </div>
            <div>
                <div v-if="datausers == null && errormessage !== null" class="alert alert-danger" role="alert">
                    {{errormessage}}
                </div>

                <div v-if="datausers == null" class="alert alert-danger" role="alert">
                    {{successmessage}}
                </div>
                <form @submit.prevent="createNewUser">
                    <div class="mb-3">
                        <label for="name" class="form-label">Nama</label>
                        <input v-model="user.name" type="test" class="form-control" id="name" >
                        
                    </div>
                    <div class="mb-3">
                        <label for="username" class="form-label">Username</label>
                        <input v-model="user.username" type="test" class="form-control" id="name" >
                    </div>
                    <button type="submit" class="btn btn-primary">Simpan</button>
                </form>
            </div>
        </layout-main>
    </div>
</template>

<script>
import LayoutMain from "@/views/LayoutMain"
export default {
    components: {
        LayoutMain
    },
    data() {
        return{
            user: { name: null, username: null},
            datausers: null,
            errormessage:null,
            successmessage: null
        }
    },
    methods: {
        createNewUser() {
            fetch("https://jsonplaceholder.typicode.com/users/",
                {
                    headers: {
                        'content-type': 'application/json; charset=UTS-8',
                    },
                    method: 'POST',
                    body: json.stringify(this.user)
                }
            )
                .then(response => response.json()) //then 1, set response sebagai json
                .then(json => {
                    if(json.id !== undefined){
                        this.datausers = json;
                        this.errormessage = "berhasil";    
                    }else{
                        this.errormessage = "gagal";
                    }
                        
                }) //then2, mengambil json dan ditampung/diset ke dalam data
                .catch(error => {
                    console.log(error);
                    this.errormessage = "silahkan coba lagi";
                })
        }
    }
}
</script>