<!-- <script>
    import AlbumTrack from "./AlbumTrack.svelte"

    export let albumTitle
    export let albumTracks

    let playing

    function setPlaying(track) {
        playing = track
    }

</script>

<h2>{albumTitle}</h2>

<ul>
    {#each albumTracks as track}
    <AlbumTrack {setPlaying} {playing} {...track} />
    {/each}
</ul> -->