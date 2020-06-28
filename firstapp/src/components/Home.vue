<template>
    <div class="container">
        <div class="row">
            <form class="form-horizontal">
                <fieldset>
                    <legend>Music App</legend>
                    <app-search></app-search>
                </fieldset>
            </form>
        </div>
        <div class="row">
            <div class="col-md-12">
               <app-result></app-result>
            </div>
        </div>
    </div>
</template>

<script>

    import Search from './Search';
    import Result from './Result';

    export default {

        components:{

            'app-result': Result,
            'app-search': Search

        }
    }

</script>