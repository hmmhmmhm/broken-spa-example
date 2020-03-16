<script lang="typescript">
    // @ts-ignore
    import * as Utils from '../utils'
    const { Logics, Components, Resources } = Utils

    // Logics
    const { } = Logics

    // Components
    const { } = Components

    // Resources
    const { } = Resources

    // Bindings
    // export let params: any = {}
    const fly = Utils.Transition.fly
    const move = () => Utils.Router.push('/b/blabla')
</script>

<!-- Page Transition Animation -->
<div
    class="bg"
    in:fly={{ y: 1000, duration: 800 }}
    out:fly={{ y: -1000, duration: 800 }}
    on:click={move}
>

    <!-- 콘텐츠 -->
    <div class="content">
    </div>
</div>

<style>
    .bg {
        position: relative;
        width: 100%;
        height: 100%;
        color: #000000;
        background-color: burlywood;
        margin: auto;
    }
    .content {
        position: relative;
        width: 100%;
        height: auto;
        /* height: calc(100% - 60px); */
        margin: 0;
        padding: 30px;
        padding-top: 40px;
        text-align: center;
    }
</style>
