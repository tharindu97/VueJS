<template>
    
     <div class="form-group">
        <label for="inputEmail" class="col-lg-2 control-label">Search music</label>
        <div class="col-lg-10">
            <input type="text" class="form-control" id="inputEmail" placeholder="search here" @input="keyPressed">
        </div>
    </div>

</template>

<script>

    import axios from 'axios'
    export default {

        methods:{

            keyPressed(event){
                var key = event.target.value
                
                axios.get('')
                .then(responce => {
                    console.log(responce.data)
                })
                .catch(e=>{
                    this.error.push(e);
                })
            }

        }
        
    }

</script>