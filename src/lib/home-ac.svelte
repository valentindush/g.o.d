<script lang="ts">
export let txt:string;

</script>
<div class="w-[10rem] text-center h-[9rem] border p-2 rounded-xl">
    <p class="text-gray-700 text-4xl font-medium">{txt.split("|")[0]}</p>
    <p class="text-lg text-gray-800 mt-6">{txt.split("|")[1]}</p>
</div>