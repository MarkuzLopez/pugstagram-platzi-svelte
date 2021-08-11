<script>
    import Profile from './Profile.svelte';
    import Stories from './Stories.svelte';
    import Footer from './Footer.svelte';

    export let nickname;
    export let name;
</script>

<!-- Sidebar.svelte -->
<style>
    .Sidebar {
      position: relative;
      padding: 6.5em 0 0 0;
      flex: 1;
      display: flex;
      flex-direction: column;
    }
    .Sidebar-container {
      position: relative;
    }
</style>

<div class="Sidebar">
    <div class="Sidebar-container">
        <Profile {nickname} {name} />
        <Stories />
        <Footer />
    </div>
</div>