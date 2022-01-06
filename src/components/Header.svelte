<script>
    import { Router, Link } from 'svelte-routing';
</script>

<div>
    <Router>
        <Link to="/">Home</Link>
        <Link to="about">About</Link>
        <Link to="create">Create</Link>  
      </Router>
</div>