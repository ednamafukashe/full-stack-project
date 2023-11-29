<script>
    import TodoItem from "$lib/todo-item.svelte";
    
const title="Todo| New";
</script>
<svelte:head>
    <link rel="stylesheet" href="main.css">
    <title>{title}</title>
</svelte:head>
<h1>{title} </h1>
<p>+ tap to add a todo</p>
<form action="" method=""  >
    <input type="text" name="text" placeholder="+ type to add a todo" >

</form>
<TodoItem/>
<TodoItem/>
<TodoItem/>