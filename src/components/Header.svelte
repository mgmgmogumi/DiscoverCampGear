<script>
    import { Router, Link } from 'svelte-routing';
</script>

<div>
    <Router>
        <Link to="/">検索</Link>
        <Link to="create">特集</Link>
        <Link to="about">About</Link>
      </Router>
</div>