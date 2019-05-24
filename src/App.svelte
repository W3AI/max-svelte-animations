<script>
    import { writable } from 'svelte/store';
    import { tweened } from 'svelte/motion';

    const progress = tweened(0);

    setTimeout(() => {
        progress.set(.5);
    }, 1500);
</script>

<progress value={$progress}></progress>



