<script>
    import {AppShell} from "@skeletonlabs/skeleton";
    import Options from "$lib/Options.svelte";
</script>

<AppShell>
    <!-- (header) -->
    <svelte:fragment slot="sidebarLeft">

        <Options />

    </svelte:fragment>
    <!-- (sidebarRight) -->
    <!-- (pageHeader) -->
    <!-- Router Slot -->
    <slot />
    <!-- ---- / ---- -->
    <!-- (pageFooter) -->
    <!-- (footer) -->
</AppShell>