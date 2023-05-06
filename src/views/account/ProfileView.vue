<template>
    <div class="container max-w-4xl mx-auto flex">
        <div class="w-1/3">
            <img src="https://placehold.co/500"
                class="w-full rounded-lg h-auto shadow-lg"
            alt="Profile Pic">
        </div>
        <div class="w-full pl-4">
            <div class="flex">
                <div class="w-1/2">
                    <h1 class="text-2xl md:text-4xl text-left text-gray-900">
                        S.Kein
                    </h1>
                    <span class="text-md text-gray-700">
                        <i><b>Mandalay, Myanmar</b></i>
                    </span>
                </div>
                <div class="w-1/2 mt-2">
                    <RouterLinkButton
                    class="float-right text-gray-900"
                    btnText="Edit Profile"
                    color="green"
                    url="edit-profile"
                    >
                    </RouterLinkButton>
                </div>

            </div>
            <ProfileInfoSection></ProfileInfoSection>
            <ProfileAboutSection></ProfileAboutSection>
        </div>
    </div>
    <SongsSection></SongsSection>
    <YoutubeVideoSection></YoutubeVideoSection>
    <PostSection></PostSection>
</template>

<script setup>
    import ProfileAboutSection from '@/components/partials/profile/ProfileAboutSection.vue';
    import ProfileInfoSection from '@/components/partials/profile/ProfileInfoSection.vue';
    import RouterLinkButton from '@/components/global/RouterLinkButton.vue';
    import SongsSection from '@/components/partials/profile/SongsSection.vue';
    import YoutubeVideoSection from '@/components/partials/profile/YoutubeVideoSection.vue';
    import PostSection from '@/components/partials/profile/PostSection.vue';
</script>

<style lang="stylus" scoped>

</style>
