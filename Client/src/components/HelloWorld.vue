<template>
  <div class="hello">
    <v-container
      fluid
      grid-list-lg
    >
      <v-layout row wrap>
            <v-flex xs4>
              <v-card color="cyan darken-2" class="white--text">
              <v-layout>
                <v-flex xs5>
                  <v-img
                    src="https://nerdsverse.files.wordpress.com/2015/07/one-piece-main-characters.png"
                    height="125px"
                    contain
                  ></v-img>
                </v-flex>
                <v-flex xs7>
                  <v-card-title primary-title>
                    <div>
                      <div class="headline">One Piece</div>
                      <div>Eichiro Oda</div>
                      <div>(1997)</div>
                    </div>
                  </v-card-title>
                </v-flex>
              </v-layout>
              <v-divider light></v-divider>
              <v-card-actions>
                <v-btn flat dark>Cek sekarang</v-btn>
              </v-card-actions>
            </v-card>
            </v-flex>
            <v-flex xs4>
              <v-card color="cyan darken-2" class="white--text">
              <v-layout>
                <v-flex xs5>
                  <v-img
                    src="http://pluspng.com/img-png/dragon-ball-png-dragon-ball-super-png-hd-750.png"
                    height="125px"
                    contain
                  ></v-img>
                </v-flex>
                <v-flex xs7>
                  <v-card-title primary-title>
                    <div>
                      <div class="headline">Dragon Ball</div>
                      <div>Akira Toriyama</div>
                      <div>(1984)</div>
                    </div>
                  </v-card-title>
                </v-flex>
              </v-layout>
              <v-divider light></v-divider>
              <v-card-actions>
                <v-btn flat dark>Cek sekarang</v-btn>
              </v-card-actions>
            </v-card>
            </v-flex><v-flex xs4>
              <v-card color="cyan darken-2" class="white--text">
              <v-layout>
                <v-flex xs5>
                  <v-img
                    src="https://static.bandainamcoent.eu/high/naruto/naruto-ultimate-ninja-blazing/00-page-setup/nb_image_description.png"
                    height="125px"
                    contain
                  ></v-img>
                </v-flex>
                <v-flex xs7>
                  <v-card-title primary-title>
                    <div>
                      <div class="headline">Naruto</div>
                      <div>Masashi Kishimoto</div>
                      <div>(2002)</div>
                    </div>
                  </v-card-title>
                </v-flex>
              </v-layout>
              <v-divider light></v-divider>
              <v-card-actions>
                <v-btn flat dark>Cek sekarang</v-btn>
              </v-card-actions>
            </v-card>
            </v-flex>

            <v-flex xs4>
            <v-card color="purple" class="white--text">
              <v-layout row>
                <v-flex xs7>
                  <v-card-title primary-title>
                    <div>
                      <div class="headline">Hunter x Hunter</div>
                      <div>Yoshihiro Togashi</div>
                      <div>(2011)</div>
                    </div>
                  </v-card-title>
                </v-flex>
                <v-flex xs5>
                  <v-img
                    src="https://i.pinimg.com/originals/4a/85/8b/4a858be38b924452847855b8ec9446e4.png"
                    height="125px"
                    contain
                  ></v-img>
                </v-flex>
              </v-layout>
              <v-divider light></v-divider>
              <v-card-actions>
                <v-btn flat dark>Cek sekarang</v-btn>
              </v-card-actions>
            </v-card>
          </v-flex>
            <v-flex xs4>
            <v-card color="purple" class="white--text">
              <v-layout row>
                <v-flex xs7>
                  <v-card-title primary-title>
                    <div>
                      <div class="headline">Tokyo Ghoul</div>
                      <div>Sui Ishida</div>
                      <div>(2012)</div>
                    </div>
                  </v-card-title>
                </v-flex>
                <v-flex xs5>
                  <v-img
                    src="https://orig00.deviantart.net/3481/f/2017/354/4/9/tokyo_ghoul_re___anime_icon_by_kiddblaster-dbxa5xw.png"
                    height="125px"
                    contain
                  ></v-img>
                </v-flex>
              </v-layout>
              <v-divider light></v-divider>
              <v-card-actions>
                <v-btn flat dark>Cek sekarang</v-btn>
              </v-card-actions>
            </v-card>
          </v-flex>
            <v-flex xs4>
            <v-hover>
            <v-card color="purple" class="white--text">
              <v-layout row>
                <v-flex xs7>
                  <v-card-title primary-title>
                    <div>
                      <div class="headline">Nanatsu no Taizai</div>
                      <div>Nakaba Suzuki</div>
                      <div>(2012)</div>
                    </div>
                  </v-card-title>
                </v-flex>
                <v-flex xs5>
                  <v-img
                    src="http://3.bp.blogspot.com/-rVkxU9IzKVA/VRqS8WvuZaI/AAAAAAAAARk/n-YgmqA2Ml8/s1600/Chapter_95_Render.png"
                    height="125px"
                    contain
                  ></v-img>
                </v-flex>
              </v-layout>
              <v-divider light></v-divider>
              <v-card-actions>
                <v-btn flat dark>Cek sekarang</v-btn>
              </v-card-actions>
            </v-card>
            </v-hover>
          </v-flex>
      </v-layout>
      <v-card v-for="category in categories" :key="category">
        <v-card-title>{{ category }}</v-card-title>
      </v-card>
    </v-container>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  props: {
    msg: String
  },
  data() {
    return{
      categories: [
        
        'Dragon Ball',
        'Naruto',
      ],
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
