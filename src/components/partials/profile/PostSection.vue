<template>
    <div class="">
        <div class="mx-auto py-4">

            <div class="flex flex-wrap font-bold text-gray-100">
                <div class="text-gray-900 text-xl">Posts</div>
                <div class="bg-green-500 w-full h-1"></div>
                <div class="w-full mt-4">                    
                    <RouterLinkButton
                    class=""
                    btnText="Create Post"
                    color="green"
                    url="account/create-post"
                    />
                   
                </div>
            </div>
        </div>
        <div class="">
        </div>
        <div class="flex flex-wrap mb-4">
            <div class="my-1 px-1 w-full md:w-1/2 lg:w-1/2">

            <div class=" border rounded-lg">
                <a href="#">
                    <img class="rounded-t-lg" src="https://placehold.co/500x300" alt="" />
                </a>
                <div class="p-2 md:p4">
                    <div class="text-lg">
                        <router-link
                        to=""
                        class="
                            underline
                            text-blue-500
                            hover:text-blue-600
                        "
                        >
                            Test Title
                        </router-link>
                    </div>
                    <p class="py-2">Location: somewhere</p>
                    <p class="text-gray-darker text-md">
                        Lorem ipsum, dolor sit amet consectetur adipisicing elit. Officia ullam iste iusto pariatur fugiat magni dicta? Consequuntur minima, esse optio maxime explicabo magnam, aut repellendus iste totam quis aperiam deleniti?
                    </p>
                    <div class="mt-2 flex items-center justify-end">
                        <router-link
                        to=""
                        class="
                            
                            bg-blue-500
                            hover:bg-blue-700
                            text-white
                            text-sm
                            font-bold
                            py-1
                            px-2
                            rounded-full
                            me-5
                        "
                        >
                            Edit Post
                        </router-link>
                        <button
                        class="
                            
                            bg-red-500
                            hover:bg-red-700
                            text-white
                            text-sm
                            font-bold
                            py-1
                            px-2
                            rounded-full
                        "
                        >
                            Delete Post
                        </button>

                    </div>
                </div>
            </div>

            </div>
        </div>
    </div>
</template>

<script setup>
    import RouterLinkButton from '../../global/RouterLinkButton.vue';

</script>