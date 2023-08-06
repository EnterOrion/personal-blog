<script lang="ts">
  import type { PageData } from "../../post/[slug]/$types";

  export let data: App.PageData;
</script>

<h1>{data.title}</h1>
<div>{@html data.content}</div>
