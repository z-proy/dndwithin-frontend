<script lang="ts">
    import {Form, Input} from 'spaper'
    // your script goes here
    export let Name: string
    export let Value: number
    let bonus = Value/2-5
    let sign: string = ""
    if (bonus > 0) {
        sign = "+"
        bonus = Math.floor(bonus)
    } else {
        bonus = Math.ceil(bonus)
    }
</script>

<main>
    <div class="attrBlock">
        <h4>{Name} ({sign}{bonus})</h4>
        <div class="child-borders">
            <div class="border-primary numBlock"><p>{Value}</p></div>
        </div>
    </div>
</main>

<style>
    .numBlock {
        width: 65px;
        text-align: center;
    }
    .attrBlock{
        width: 80px;
        padding-left: 40px;
        padding-right: 40px;
    }
    main {
        text-align: center;
    }
    h4 {
        margin-top: 0px;
        margin-bottom: 0px;;
    }
    /* your styles go here */
</style>