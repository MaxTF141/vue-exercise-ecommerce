<template>
    <div class="row justify-content-center">
        <div class="col-4 form-container mt-5">
            <h2 class="text-center text-white">Contact Us</h2>
            <form>
                <div class="mb-3">
                    <label for="exampleInputPassword1" class="form-label text-white">Name</label>
                    <input type="text" class="form-control" id="exampleInputPassword1" placeholder="Name" v-model="fullName"/>
                </div>
                <div class="mb-3">
                    <label for="exampleInputPassword1" class="form-label text-white">Surname</label>
                    <input type="text" class="form-control" id="exampleInputPassword1" placeholder="Surname" v-model="surname"/>
                </div>
                <div class="mb-3">
                    <label for="exampleInputPassword1" class="form-label text-white">Email</label>
                    <input type="text" class="form-control" id="exampleInputPassword1" placeholder="Email Address" v-model="email"/>
                </div>
                <div class="mb-3 d-flex flex-column">
                    <label for="message" class="text-white">
                        Message:
                    </label>
                    <textarea id="message" name="message" rows="5" cols="30" required></textarea>
                </div>
                <button type="submit" class="btn btn-primary" v-on:click.prevent="submit">Sign In</button>
            </form>
        </div>
    </div>
</template>
<script>
export default {
    methods:{
        submit(){
                alert(`${this.fullName} ${this.surname} with the email ${this.email}. We've received your information and will contact you by email.`)
            }
    }

};
</script>
<style scoped>
.form-container {
    border-radius: 30px;
    border: 1px solid darkcyan;
    box-shadow: inset 1px 1px 8px black;
    padding: 30px;
}

.center {
    text-align: center;
}
</style>
