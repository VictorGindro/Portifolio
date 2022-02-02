<template>

    <v-carousel  cycle height="600"  show-arrows-on-hover>
        <v-carousel-item v-for="(slide, i) in slides" :key="i" eager>
            <v-parallax v-if="i==0" dark height="600" src="../assets/codigos.png">
                <v-row align="center"  justify="center">
                    <v-col class="text-center " cols="12">
                        <h1 class="mb-4 font-weight-black ">
                            Mean Stack Dev
                        </h1>
                        <h4 class="font-weight-black ">
                            Multi-language Experience <br />
                            Java / C# / C++ / NodeJs <br />
                            Diverse Framework Knowledge across multiple langages
                        </h4>
                    </v-col>
                </v-row>
            </v-parallax>
            <v-parallax v-if="i==1" dark height="600" src="../assets/Brain.jpg">
                <v-row align="center" justify="center">
                    <v-col class="text-center" cols="12">
                        <h1 class="mb-4 font-weight-black white--text">
                            Data Managing
                        </h1>
                        <h3 class="font-weight-black white--text">
                            ChatBot Experience with Cisco Webex and Discord APIs<br />
                            Oracle SQL / PLSQL and MongoDB experience <br />

                        </h3>
                    </v-col>
                </v-row>
            </v-parallax>
            <v-parallax v-if="i==2" height="600" dark src="../assets/collab2.png">
                <v-row align="center" justify="center">
                    <v-col class="text-center font-weight-black" cols="12">
                        <h1 class="mb-4 font-weight-black text">
                            Collaboration Specialist
                        </h1>
                        <h3 class="font-weight-black">
                            Webex, MS Teams, Discord <br/>
                            A diverse experience with collaboration devices
                        </h3>
                    </v-col>
                </v-row>
            </v-parallax>
            <v-parallax v-if="i==3" height="600" dark src="../assets/mobile.png">
                <v-row align="center" justify="center">
                    <v-col class="text-center font-weight-black" cols="12">
                        <h1 class="mb-4 font-weight-black ">
                            Mobile Dev skills
                        </h1>
                        <h3 class=" font-weight-black ">
                            Native Androis and IOS Developing <br/>
                            Hybrid coding with vue.JS and Electron/Ionic
                        </h3>
                    </v-col>
                </v-row>
            </v-parallax>
        </v-carousel-item>
    </v-carousel>
</template>
<script>
    export default {
        data: () => ({
            slides: 4,
        })
    }
</script>
