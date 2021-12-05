<template>
  <div id="app">
    <section class="has-text-centered background hero is-fullheight">
      <div class="musicheading has-text-success-light is-size-1">
        mymusic
      </div>
      <div class="musicimage">
        <figure class="image is-128x128">
          <img
            class="is-rounded"
            src="data:image/jpeg;base64,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"
          />
        </figure>
      </div>
      <div class="is-size-3 has-text-warning-light">
        {{ currentsong.title }} <br />
        Singer: {{ currentsong.artist }}
      </div>
      <div class="controls">
        <button class="button is-primary is-rounded" @click="prev()">
          <i class="fas fa-backward"></i>
        </button>
        &nbsp;
        <button
          v-if="isplaying"
          class="button is-primary is-rounded"
          @click="playsong(currentsong.src)"
        >
          <i class="fas fa-play"></i>
        </button>
        <button
          v-else
          key="fa-pause"
          class="button is-primary is-rounded"
          @click="pause()"
        >
          <i class="fas fa-pause"></i>
        </button>
        <button class="button is-primary is-rounded" @click="next()">
          <i class="fas fa-forward"></i>
        </button>
      </div>
      <div v-if="hideplaylist" @click="hiddeplaylist()">
        <button class="button is-black is-rounded ">colseplaylist</button>
      </div>
      <div v-else @click="playlist()">
        <button class="button is-black is-rounded">openplaylist</button>
      </div>
      <div v-if="playlist1">
        <strong>playlist</strong>
        <div
          v-for="song in songs"
          :key="song"
          @click="playsong(song)"
          style="padding:1vh;"
        >
          <button class="button is-black ">
            {{ song.title }}---{{ song.artist }}
          </button>
        </div>
      </div>
    </section>
  </div>
</template>

<script>
export default {
  name: "app",
  data() {
    return {
      currentsong: {},
      isplaying: true,
      playlist1: false,
      index: 0,
      hideplaylist: false,
      songs: [
        {
          title: "Inkem-Inkem",
          artist: "sid-sriram",
          src: "/public/01.mp3"
        },

        {
          title: "jersey",
          artist: "DSP",
          src: "/public/02.mp3"
        },

        {
          title: "U-turn",
          artist: "thaman",
          src: "/public/03.mp3"
        },

        {
          title: "Anaganaganaga..",
          artist: "ManiSharma",
          src: "/public/04.mp3"
        }
      ],
      player: new Audio()
    };
  },
  created() {
    this.currentsong = this.songs[this.index];
    this.player.src = this.currentsong.src;
  },
  methods: {
    playsong(song) {
      //var player = new Audio(src)
      if (typeof song.src != "undefined") {
        this.currentplayer = song;
        this.player.src = this.currentplayer.src;
      }
      this.player.play();
      this.isplaying = false;
    },
    pause() {
      this.player.pause();
      this.isplaying = true;
    },
    playlist() {
      this.playlist1 = true;
      this.hideplaylist = true;
    },
    next() {
      this.index++;
      if (this.index > this.songs.length - 1) {
        this.index = 0;
      }
      this.currentsong = this.songs[this.index];
      this.player.src = this.currentsong.src;
      this.player.play();
      this.isplaying = false;
    },
    prev() {
      this.index--;
      if (this.index < 0) {
        this.index = this.songs.length - 1;
      }
      this.currentsong = this.songs[this.index];
      this.player.src = this.currentsong.src;
      this.player.play();
      this.isplaying = false;
    },
    hiddeplaylist() {
      this.playlist1 = false;
      this.hideplaylist = false;
    }
  }
};
</script>

<style>
.controls {
  padding-bottom: 5%;
}
</style>
