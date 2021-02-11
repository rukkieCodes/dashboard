<template>
  <div class="dashboard">
    <div class="all_sections">
      <nav class="nav_bar">
        <div class="left_side">
          <div class="left_elements">
            <div class="inputs">
              <div class="input">
                <span class="mdi mdi-magnify"></span>
                <input type="text" placeholder="Search" />
              </div>
            </div>
            <div class="buttons">
              <button class="btn ripple">Post a Task</button>
              <button class="btn ripple">Browse tasks</button>
              <button class="btn ripple">My Tasks</button>
              <button class="btn ripple">Profile</button>
            </div>
          </div>
        </div>
        <div class="right_side">
          <div class="buttons">
            <router-link to="/" class="btn">Help</router-link>
            <router-link to="/" class="btn">Notifications</router-link>
            <router-link to="/" class="btn">Messages</router-link>
          </div>

          <div class="avatar">
            <div class="img">
              <img src="../assets/images/john.jpg" alt="AVATAR" />
            </div>
          </div>

          <div class="cog">
            <button>
              <span class="mdi mdi-cog"></span>
            </button>
          </div>
        </div>
      </nav>

      <aside class="drawer">
        <div class="content">
          <div class="menu_btn">
            <button><i class="mdi mdi-menu"></i></button>
          </div>
          <div class="buttons">
            <button><span class="mdi mdi-view-dashboard"></span></button>
            <button><span class="mdi mdi-wallet"></span></button>
            <button><img src="../assets/images/stars.svg" alt="" /></button>
            <button><span class="mdi mdi-bell-ring"></span></button>
            <button><span class="mdi mdi-clipboard-alert"></span></button>
            <button><span class="mdi mdi-account-plus"></span></button>
            <button><span class="mdi mdi-help-circle"></span></button>
          </div>
        </div>
      </aside>

      <main class="main_section">
        <div class="main_section_content">
          <div class="section_one">
            <div class="content">
              <div class="left_side">
                <button class="help_btn">
                  <span class="mdi mdi-help"></span>
                </button>

                <div class="card">
                  <div class="content">
                    <div class="avatar">
                      <span class="mdi mdi-cube-send"></span>
                    </div>

                    <p class="p1">Post a Task</p>

                    <p class="p2">
                      Lorem ipsum dolor sit amet consectetur adipisicing elit.
                    </p>
                  </div>
                </div>

                <div class="seprator"></div>

                <div class="right_avatars">
                  <div class="avatars">
                    <div v-for="(avatar, index) in first_avatars" :key="index" class="box">
                      <div class="avatar">
                        <img :src="avatar.image" alt="" />
                      </div>
                      <p class="p1">{{ avatar.title }}</p>
                    </div>
                    <div class="box">
                      <div class="avatar">
                        <img src="../assets/images/705.svg" alt="" />
                      </div>
                      <p class="p1">Translate</p>
                    </div>
                    <div class="box">
                      <div class="avatar">
                        <img src="../assets/images/716.svg" alt="" />
                      </div>
                      <p class="p1">Graphic</p>
                    </div>
                    <div class="box">
                      <div class="avatar">
                        <img src="../assets/images/715.svg" alt="" />
                      </div>
                      <p class="p1">Education</p>
                    </div>
                    <div class="box">
                      <div class="avatar">
                        <img src="../assets/images/708.svg" alt="" />
                      </div>
                      <p class="p1">Marketing</p>
                    </div>
                    <div class="box">
                      <div class="avatar">
                        <img
                          class="delivery"
                          src="../assets/images/664.svg"
                          alt=""
                        />
                      </div>
                      <p class="p1">Delivery</p>
                    </div>
                    <div class="box">
                      <div class="avatar">
                        <img src="../assets/images/714.svg" alt="" />
                      </div>
                      <p class="p1">Home</p>
                    </div>
                    <div class="box">
                      <div class="avatar">
                        <img src="../assets/images/713.svg" alt="" />
                      </div>
                      <p class="p1">Handyman</p>
                    </div>
                    <div class="box">
                      <div class="avatar">
                        <img src="../assets/images/712.svg" alt="" />
                      </div>
                      <p class="p1">Car</p>
                    </div>
                    <div class="box">
                      <div class="avatar">
                        <img src="../assets/images/711.svg" alt="" />
                      </div>
                      <p class="p1">Nursing</p>
                    </div>
                    <div class="box">
                      <div class="avatar">
                        <img src="../assets/images/710.svg" alt="" />
                      </div>
                      <p class="p1">Ceremonies</p>
                    </div>
                    <div class="box">
                      <div class="avatar">
                        <img src="../assets/images/709.svg" alt="" />
                      </div>
                      <p class="p1">Other</p>
                    </div>
                  </div>
                </div>
              </div>

              <div class="right_side">
                <button class="float">
                  <span class="mdi mdi-circle-edit-outline"></span>
                </button>
                <div class="content">
                  <button class="help_btn">
                    <span class="mdi mdi-help"></span>
                  </button>

                  <div class="avatar_section">
                    <div class="avatar">
                      <span class="mdi mdi-account-alert"></span>
                    </div>
                    <p>Profile Status</p>
                  </div>

                  <div class="marks">
                    <div class="left_side">
                      <div class="text">
                        <span class="mdi mdi-check"></span>
                        <p>Account</p>
                      </div>
                      <div class="text">
                        <span class="mdi mdi-check"></span>
                        <p>Profile</p>
                      </div>
                    </div>
                    <div class="right_side">
                      <div class="text">
                        <span class="mdi mdi-close"></span>
                        <p>Verification</p>
                      </div>
                      <div class="text">
                        <span class="mdi mdi-close"></span>
                        <p>Payments</p>
                      </div>
                    </div>
                  </div>
                </div>
              </div>
            </div>
          </div>

          <div class="section_two">
            <div class="content">
              <div class="heading">
                <h1>My Task summary</h1>
              </div>
              <div class="sides">
                <div class="left_side">
                  <div class="content">
                    <div class="left">
                      <div class="item">
                        <p>Draft</p>
                      </div>
                      <div class="item">
                        <p>Open for offer</p>
                      </div>
                      <div class="item">
                        <p>Open for offer</p>
                      </div>
                      <div class="item">
                        <p>Assigned</p>
                        <p>+1</p>
                      </div>
                      <div class="item">
                        <p>Awaiting Payment</p>
                        <p>+1</p>
                      </div>
                      <div class="item">
                        <p>Reviews</p>
                      </div>
                      <div class="item">
                        <p>Completed</p>
                        <p>+1</p>
                      </div>
                    </div>

                    <div class="seperator"></div>

                    <div class="right">
                      <h1>34</h1>
                      <p>Total amount</p>
                      <p>+2 in the last 30 days</p>
                    </div>
                  </div>
                </div>
                <div class="right_side">
                  <img src="../assets/images/sparkline.png" alt="">
                </div>
              </div>
            </div>
          </div>

          <div class="section_three">
            <div class="content">
              <div class="left_side">
                <div class="card">
                  <div class="avatar">
                    <span class="mdi mdi-bell-ring"></span>
                  </div>

                  <p>Notifications</p>
                  <p>+2 in the last Hour</p>
                </div>
              </div>

              <div class="right_side">
                <div class="card">
                  <div class="avatar">
                    <span class="mdi mdi-account-group"></span>
                  </div>

                  <p>Refar a friend</p>
                  <p>
                    Lorem ipsum dolor sit amet consectetur adipisicing elit.
                  </p>
                </div>
              </div>
            </div>
          </div>

          <div class="section_four">
            <div class="content">
              <div class="full">
                <div class="card">
                  <div class="avatar">
                    <span class="mdi mdi-bullhorn"></span>
                  </div>

                  <p>Announcment</p>
                  <p>
                    Lorem ipsum dolor sit amet consectetur adipisicing elit.
                  </p>
                </div>
              </div>
            </div>
          </div>

          <div class="section_five">
            <div class="content">
              <div class="cards">
                <div class="main_card">
                  <div class="avatar">
                    <span class="mdi mdi-bullhorn"></span>
                  </div>

                  <p>Announcment</p>
                  <p>
                    Lorem ipsum dolor sit amet consectetur adipisicing elit.
                  </p>
                </div>

                <div class="sub_cards">
                  <div class="card">
                    <div class="head">
                      <div class="left">
                        <div class="avatar">
                          <img src="../assets/images/john.jpg" alt="" />
                        </div>
                        <p>Name Name</p>
                      </div>

                      <div class="right">
                        <p>5 minutes ago</p>
                      </div>
                    </div>

                    <div class="body"></div>

                    <div class="foot">
                      <div class="left">
                        <p>1 Offer</p>
                        <p>2 Ticker</p>
                      </div>
                      <div class="right">
                        <p>Online</p>
                      </div>
                    </div>
                  </div>
                  <div class="card">
                    <div class="head">
                      <div class="left">
                        <div class="avatar">
                          <img src="../assets/images/john.jpg" alt="" />
                        </div>
                        <p>Name Name</p>
                      </div>

                      <div class="right">
                        <p>5 minutes ago</p>
                      </div>
                    </div>

                    <div class="body"></div>

                    <div class="foot">
                      <div class="left">
                        <p>1 Offer</p>
                        <p>2 Ticker</p>
                      </div>
                      <div class="right">
                        <p>Online</p>
                      </div>
                    </div>
                  </div>
                  <div class="card">
                    <div class="head">
                      <div class="left">
                        <div class="avatar">
                          <img src="../assets/images/john.jpg" alt="" />
                        </div>
                        <p>Name Name</p>
                      </div>

                      <div class="right">
                        <p>5 minutes ago</p>
                      </div>
                    </div>

                    <div class="body"></div>

                    <div class="foot">
                      <div class="left">
                        <p>1 Offer</p>
                        <p>2 Ticker</p>
                      </div>
                      <div class="right">
                        <p>Online</p>
                      </div>
                    </div>
                  </div>
                </div>
              </div>
            </div>
          </div>
        </div>
      </main>
    </div>
  </div>
</template>

<script>
export default {
  name: "Dashboard",
};
</script>

<style lang="scss" scoped>
@import url(../assets/addons/icon/css/materialdesignicons.css);
@import "../assets/style/dashboard.scss";
</style>