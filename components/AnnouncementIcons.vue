<template>
    <div class="mb-3">
        <b-avatar 
            variant="primary" 
            size="1.3rem" 
            src="~static/icons/metro-pin.svg" 
            v-b-tooltip.hover.bottomright 
            title="Pin Announcement"
        ></b-avatar>
        <b-avatar 
            variant="primary" 
            size="1.3rem" 
            icon="share-fill" 
            v-b-tooltip.hover.bottomright 
            title="Share Timeline"
        ></b-avatar>
        <b-avatar 
            variant="primary" 
            size="1.3rem" 
            icon="pencil-square" 
            v-b-tooltip.hover.bottomright 
            title="Edit Announcement"
        ></b-avatar>
    </div>
</template>