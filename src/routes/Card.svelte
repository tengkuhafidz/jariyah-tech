<script lang="ts">
    export let title: string
    export let image: string
    export let description: string
    export let tags: string
    export let url: string
</script>

<div>
    <a href={url} target="_blank" rel="noreferrer">
        <h2 class="font-branding text-2xl pb-4 font-bold hover:text-teal-400 cursor-pointer">
            {title}
        </h2>
    </a>
    <a href={url} target="_blank" rel="noreferrer">
        <img src={image} alt="{title} banner" class="hover:scale-105 hover:shadow-2xl rounded-md duration-500 cursor-pointer" />
    </a>
    <div class="py-4">
        <p class="font-light leading-tight">{description}</p>
        <p class="text-teal-400 font-branding text-sm mt-1">{tags}</p>
    </div>
</div>