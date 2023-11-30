<script>
    import TodoItem from "$lib/todo-item.svelte";
    
    
const title="Todo| New";
</script>

<style>
    p{
        font-size: 1.2rem;
        text-align: center;
    }
    .todos{
        width: 100%;
        max-width: 42rem;
        margin: 4rem auto 0 auto;
    }
    .todo-text{
        width:100%;

    }
    .todo-text input{
       font-size: 28px;
       width:100%; 
       padding: 0 0 0.5rem 1em;
       box-sizing: border-box;
       background: rgb(255, 255,255, 0.05);
       border-radius: 8px;
       text-align: center;
      
    }
    .todos :global(input){
      border: 1px solid transparent;
    }

    .todos :global(input:focus-visible){
        outline: none;
        box-shadow: inset 1px 1px 6px rgb(0, 0,0, 0.1);
        border: 1px solid #ff3e00;
    }
</style>
<svelte:head>
    <link rel="stylesheet" href="main.css">
    <title>{title}</title>
</svelte:head>

<div class="todos">
    <h1>{title} </h1>
    
    <form class="todo-text" action="" method=""  >
        <input type="text" name="text" placeholder="+ type to add a todo" >
    </form>

<TodoItem/>
<TodoItem/>
<TodoItem/>
</div>