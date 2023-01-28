<script lang="ts">

    export let texto: string;
    export let triplo: boolean = false;
    export let duplo: boolean = false;
    export let operacao: boolean = false;
    export let destaque: boolean = false;
    export let onClick: (valor: string) => void = () => {}

    function click(){
        console.log('click')
    }

</script>

<button 
    on:click={() => { onClick(texto)}}
    class="botao" class:triplo class:duplo class:operacao class:destaque>
    {texto}
</button>

<style>
    .botao{     
        margin: 0;
        border: 1px solid var(--cor-fundo);
        flex-basis: 25%;
        cursor: pointer
    }

    .botao:hover{
        opacity: 0.8;
    }

    .triplo{
        flex-basis: 75%;
    }

    .duplo{
        flex-basis: 50%;
    }

    .operacao{
        background-color: orange;
        color: white;
    }

    .destaque{
        background-color: red;
        color: white;
         
    }
</style>