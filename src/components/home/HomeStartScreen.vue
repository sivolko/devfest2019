<template>
    <v-container fluid class="my-4">
        <v-layout wrap align-center justify-center row fill-height class="py-5">
            <v-flex xs12 sm7 md7 lg7 xl7 class="px-5 py-5">
                <v-img
                    :src="require('@/assets/img/logo.webp')"
                    :lazy-src="require('@/assets/img/logo.webp')"
                    width="40vh">
                    <v-layout
                        slot="placeholder"
                        fill-height
                        align-center
                        justify-center
                        ma-0
                    >
                        <v-progress-circular indeterminate color="grey lighten-5"></v-progress-circular>
                    </v-layout>
                </v-img>
                <!-- <p class="google-font mb-1" style="font-weight: 350;color: #616161;font-size:300%"><b>DevFest  
                    <span style="color: #1a73e8;">Punjab</span>.</b> 
                </p> -->
               
                <p class="google-font mb-0 mt-5 mb-1" style="font-size:140%">GDG Jalandhar <v-icon>mdi-unfold-more-vertical mdi-36px</v-icon> GDG Chandigarh</p>
                <p class="google-font mb-0" style="font-size:100%">DevFests are community-led, developer events hosted by GDG chapters around the globe focused on community building and learning about Google’s technologies. </p>
                <p class="google-font my-0 my-3 mt-5" >
                    <span style="font-size:100%;color:#424242;border:1px solid indigo;border-radius:8px" class="pa-2">
                        The LaLit Chandigarh | 28th September, 2019
                    </span>
                </p> 
                <p class="google-font mt-5" style="font-size:110%;color:#9e9e9e">
                    <span v-for="(item,i) in chapterDetails.ChapterHashTags" :key="i">
                        #{{item}} &nbsp;
                    </span>
                </p>

                <!-- <v-btn aria-label="Registration Button" disabled  target="_blank" class="ma-0 google-font elevation-1" color="#1a73e8" style="text-transform: capitalize;border-radius:5px;color:white">Registration Closed</v-btn> -->

                
            </v-flex>
           <v-flex xs12 sm5 md3 lg5 xl5 class="text-xs-center ">
                <v-img
                    :src="require('@/assets/img/bg.png')"
                    :lazy-src="require('@/assets/img/bg.png')"
                    width="100%">
                    <v-layout
                        slot="placeholder"
                        fill-height
                        align-center
                        justify-center
                        ma-0
                    >
                        <v-progress-circular indeterminate color="grey lighten-5"></v-progress-circular>
                    </v-layout>
                </v-img>
            </v-flex> 
        </v-layout>
        <!-- <v-layout wrap align-center justify-center row fill-height  >
           <v-flex xs12 sm5 md3 lg4 xl4 class="text-xs-center ">
                <v-img
                    :src="require('@/assets/img/main.webp')"
                    :lazy-src="require('@/assets/img/main.webp')"
                    width="100%">
                    <v-layout
                        slot="placeholder"
                        fill-height
                        align-center
                        justify-center
                        ma-0
                    >
                        <v-progress-circular indeterminate color="grey lighten-5"></v-progress-circular>
                    </v-layout>
                </v-img>
            </v-flex> 
            <v-flex xs12 sm7 md8 lg8 xl8 class="px-5">
                <p class="google-font mb-1" style="font-weight: 350;color: #616161;font-size:200%"><b>DevFest  
                    <span style="color: #1a73e8;">Punjab</span>.</b> 
                </p>
               
                <p class="google-font mb-0 mt-0" style="font-size:140%">GDG Jalandhar <v-icon>mdi-unfold-more-vertical mdi-36px</v-icon> GDG Chandigarh</p>
                <p class="google-font mb-0" style="font-size:100%">DevFests are community-led, developer events hosted by GDG chapters around the globe focused on community building and learning about Google’s technologies. </p>
                <p class="google-font my-0" style="font-size:100%;color:#424242">
                    The LaLit Chandigarh | 28th September, 2019
                </p> 
                <p class="google-font" style="font-size:110%;color:#9e9e9e">
                    <span v-for="(item,i) in chapterDetails.ChapterHashTags" :key="i">
                        #{{item}} &nbsp;
                    </span>
                </p>

                <v-btn aria-label="Registration Button" disabled  target="_blank" class="ma-0 google-font elevation-1" color="#1a73e8" style="text-transform: capitalize;border-radius:5px;color:white">Registration Closed</v-btn>

           
            </v-flex>
        </v-layout> -->

    </v-container>
</template>

<script>
import ChapterDetails from '@/assets/data/chapterDetails.json'
export default {
    data() {
        return {
            chapterDetails: ChapterDetails
        }
    },
}
</script>
