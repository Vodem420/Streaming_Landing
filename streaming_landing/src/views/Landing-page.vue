<template>
    <div class="LandingPage">
        <header>
            <div class="btn btn__secondary"><span>Log in</span></div>
        </header>
        <div class="S1">
            <div class="S1__left">
                <label>It’s a hot place for your streaming fantasy.</label>
                <p>It’s a free space for watching streams and chatting with alluring people.</p>
            </div>
            <div class="S1__right">
                <div v-if="withEmail" class="S1__right__withEmail">
                    <div class="S1__right__item">
                        <img :src="$img['S1__1']" alt="Sign up with Google"/>
                        <span>Sign up with Google</span>
                    </div>
                    <div class="text">or</div>
                    <div class="inputWrapper">
                        <label>Email</label>
                        <input type="text" class="input-comp" placeholder="e.g. Alex@email.com">
                    </div>
                    <div class="inputWrapper">
                        <label>Password</label>
                        <input type="text" class="input-comp password" placeholder="8+ characters">
                        <img :src="$img['S1__3']">
                    </div>
                    <div class="S1__right__item">
                        <img :src="$img['S1__2']" class="email" alt="Sign up with Google"/>
                        <span>Sign up with Google</span>
                    </div>
                    <p>You hereby confirm that you are fully able and
                        competent to access Livebeam and comply with the
                        Terms of Use & Service, and are at least eighteen (18) 
                        years of age or the age of majority under the law of 
                        the jurisdiction of your residence and the one you are 
                        accessing Livebeam from.
                    </p>
                </div>
                <div v-if="withData" class="S1__right__withData">
                    <div class="toggleWrapper">
                        <label>I am</label>
                        <button class="btn">Male</button>
                        <button class="btn">Female</button>
                    </div>
                    <div class="inputWrapper">
                        <label>My name</label>
                        <input type="text" class="input-comp" placeholder="e.g. Alex">
                    </div>
                    <div class="inputWrapper">
                        <label>I was born</label>
                        <input type="text" class="input-comp" placeholder="MM/DD/YYYY">
                    </div>
                    <div class="rules">
                        <div></div>
                        <span>I have read understand and agree to Terms of Use,
                            Privacy Policy, Disclosures&Disclaimers.
                        </span>
                    </div>
                    <button class="btn btn__main">Sign up now</button>
                </div>
                <div class="slider">
                    <span :class="{active: withData}" @click="openEmail()"></span>
                    <span :class="{active: withEmail}" @click="openData()"></span>
                </div>
            </div>
            <div class="S1__responsiveRight">
                    <img :src="$img['S7__1']"/>
                    <div class="bxsh-circle animated"></div>
                    <button class="btn btn__main">Sign up now</button>
            </div>
            <div class="S1__right responsive">
                <div class="title">
                    <label>It’s a dedicated space for your bold fantasies!</label>
                    <p>Hundreds of attractive admirers are already waiting for you here. 
                        Don’t delay – dive into the world of streaming, flirting and hot communication right now!
                    </p>
                </div>
                <div v-if="withEmail" class="S1__right__withEmail">
                    <div class="S1__right__item">
                        <img :src="$img['S1__1']" alt="Sign up with Google"/>
                        <span>Sign up with Google</span>
                    </div>
                    <div class="text">or</div>
                    <div class="inputWrapper">
                        <label>Email</label>
                        <input type="text" class="input-comp" placeholder="e.g. Alex@email.com">
                    </div>
                    <div class="inputWrapper">
                        <label>Password</label>
                        <input type="text" class="input-comp password" placeholder="8+ characters">
                        <img :src="$img['S1__3']">
                    </div>
                    <div class="S1__right__item">
                        <img :src="$img['S1__2']" class="email" alt="Sign up with Google"/>
                        <span>Sign up with Google</span>
                    </div>
                    <p>You hereby confirm that you are fully able and
                        competent to access Livebeam and comply with the
                        Terms of Use & Service, and are at least eighteen (18) 
                        years of age or the age of majority under the law of 
                        the jurisdiction of your residence and the one you are 
                        accessing Livebeam from.
                    </p>
                </div>
                <div v-if="withData" class="S1__right__withData">
                    <div class="toggleWrapper">
                        <label>I am</label>
                        <button class="btn">Male</button>
                        <button class="btn">Female</button>
                    </div>
                    <div class="inputWrapper">
                        <label>My name</label>
                        <input type="text" class="input-comp" placeholder="e.g. Alex">
                    </div>
                    <div class="inputWrapper">
                        <label>I was born</label>
                        <input type="text" class="input-comp" placeholder="MM/DD/YYYY">
                    </div>
                    <div class="rules">
                        <div></div>
                        <span>I have read understand and agree to Terms of Use,
                            Privacy Policy, Disclosures&Disclaimers.
                        </span>
                    </div>
                    <button class="btn btn__main">Sign up now</button>
                </div>
                <div class="slider">
                    <span :class="{active: withData}" @click="openEmail()"></span>
                    <span :class="{active: withEmail}" @click="openData()"></span>
                </div>
            </div>
            <div class="bxsh-circle animated"></div>
        </div>
        <div class="S2">
            <section class="splide">
                <div class="splide__track">
                        <ul class="splide__list">
                            <li class="splide__slide"><img :src="$img['S2__1']"/></li>
                            <li class="splide__slide"><img :src="$img['S2__2']"/></li>
                            <li class="splide__slide"><img :src="$img['S2__3']"/></li>
                            <li class="splide__slide"><img :src="$img['S2__4']"/></li>
                        </ul>
                </div>
            </section>
        </div>
        <div class="S3__boxShadow">
            <div class="S3__wrapper">
                <div class="S3">
                    <label>About</label>
                    <p>It’s a global <b>streaming platform</b> for communication and meeting incredibly beautiful people. 
                        We created an excellent place where you can enjoy your time and find <b>appropriate matches</b> at first.
                    </p>
                    <p>Approximately 80% of our users have already found their lovelies. 
                        <b>Watch streams</b> without hindrance and meet someone <b>who interests you.</b>
                    </p>
                    <button class="btn btn__main">Join for free</button>
                    <div class="bxsh-circle animated"></div>
                </div>
            </div>
        </div>
        <div class="S4__wrapper">
            <div class="S4">
                <label>Why join us?</label>
                <div class="S4__top">
                    <div class="S4__item">
                        <div class="S4__item__wrapper">
                            <img :src="$img['S4__1']"/>
                            <span>Chat with attractive streamers for free</span>
                        </div>
                        <p>It’s an excellent web platform for streaming. 
                            Write messages to the beautiful streamers for free and explore this 
                            magical universe of communication!
                        </p>
                    </div>
                    <div class="S4__item">
                        <div class="S4__item__wrapper">
                            <img :src="$img['S4__2']"/>
                            <span>Only verified users</span>
                        </div>
                        <p>We care about the privacy and security of our customers. 
                            All accounts are verified so look for an attractive stranger confidently!
                        </p>
                    </div>
                    <img class="static" :src="$img['S6__4']"/>
                </div>
                <div class="S4__bottom">
                    <div class="S4__item">
                        <div class="S4__item__wrapper">
                            <img :src="$img['S4__3']"/>
                            <span>Customized search</span>
                        </div>
                        <p>Match alluring partners for your own preferences. 
                            Maybe you will be interested in a hot slender European or shy beautiful Asian? Make your choice… 
                        </p>
                    </div>
                    <div class="S4__item">
                        <div class="S4__item__wrapper">
                            <img :src="$img['S4__4']"/>
                            <span>Easy to use</span>
                        </div>
                        <p>Forget about hundreds of annoying notifications and inconvenient use. 
                            We have created the platform as easy to use and search as possible. 
                            Don’t waste your time studying functionality. Just enjoy!
                        </p>
                    </div>
                </div>
                <div class="bxsh-circle animated"></div>
            </div>
        </div>
        <div class="S5__wrapper">
            <div class="S5">
                <label>Here you can find</label>
                <div class="S5__item">
                    <img :src="$img['S5__1']"/>
                    <span>Watching streams of everyone you really like;</span>
                </div>
                <div class="S5__item">
                    <img :src="$img['S5__2']"/>
                    <span>Free communication with pretty streamers;</span>
                </div>
                <div class="S5__item">
                    <img :src="$img['S5__3']"/>
                    <span>Sweet connection with people you match;</span>
                </div>
                <div class="S5__item">
                    <img :src="$img['S5__4']"/>
                    <span>New acquaintances with someone who has similar interests;</span>
                </div>
                <div class="S5__item">
                    <img :src="$img['S5__5']"/>
                    <span>Fascinating hobbies and exciting occupations from people you fancy.</span>
                </div>
                <div class=" animated"></div>
            </div>
        </div>
        <div class="S6__wrapper">
            <div class="S6">
                <label>It’s a universe of communication and streaming without borders!</label>
                <p>Let yourself to be free – share your thoughts, delight, and fears with beautiful strangers!</p>
                <section class="splide splide2">
                    <div class="splide__track">
                        <ul class="splide__list">
                            <li class="splide__slide"><img :src="$img['S6__1']"/></li>
                            <li class="splide__slide"><img :src="$img['S6__2']"/></li>
                            <li class="splide__slide"><img :src="$img['S6__3']"/></li>
                            <li class="splide__slide"><img :src="$img['S6__4']"/></li>
                            <li class="splide__slide"><img :src="$img['S6__5']"/></li>
                        </ul>
                    </div>
                </section>
                <button class="btn btn__main static">Join for free</button>
                <button class="btn btn__main responsive">Join us for free</button>
                <div class="bxsh-circle animated"></div>
            </div>
        </div>
        <div class="S7__wrapper">
            <div class="S7">
                <div class="S7__left">
                    <label>It’s a dedicated space for your bold fantasies!</label>
                    <p>Hundreds of attractive admirers are already waiting for you here. 
                        Don’t delay – dive into the world of streaming, flirting, 
                        and hot communication right now!
                    </p>
                    <button class="btn btn__main">Write to her</button>
                </div>
                <div class="S7__right">
                    <img :src="$img['S7__1']"/>
                    <div class="bxsh-circle animated"></div>
                </div>
            </div>
        </div>
        <footer class="S8">
            <div class="S8__wrapper">
                <div class="S8__item">
                    <a>support@gmail.com</a>
                    <a>Unsubscribe</a>
                </div>
                <div class="S8__item">
                    <a>Legal terms</a>
                    <a>Terms of Use</a>
                    <a>Diclosures&Disclaimers</a>
                </div>
                <div class="S8__item">
                    <a>Privacy info</a>
                    <a>Privacy Policy</a>
                    <a>Cookie Policy</a>
                </div>
                <div class="S8__item">
                    <a>About</a>
                    <a>About Us</a>
                </div>
            </div>
        </footer>
    </div>
</template>

<script>
import Splide from '@splidejs/splide';
import '@splidejs/splide/css';
 export default {
    data() {
        return {
            withEmail: true,
            withData: false,
            slide: 0
        };
    },
    mounted(){
        var splide = new Splide( '.splide', 
            {
                type    : 'loop',
                arrows: false,
                pagination: false,
                perPage : 3,
                autoplay: true,
            },
        );
        var splide2 = new Splide( '.splide2', 
            {
                type    : 'loop',
                arrows: false,
                pagination: false,
                perPage : 3,
                autoplay: true,
            },
        );
        splide.mount();
        splide2.mount();
    },
    methods:{
        openEmail(){
            this.withEmail = true
            this.withData = false
        },
        openData(){
            this.withData = true
            this.withEmail = false
        }
    }
};
</script>