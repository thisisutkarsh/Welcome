<template>
  <div class="welcome">
    <div class="main">
      <div class="start bot">
        <div class="logo-main">
          <img src="./assets/logo-click.png" alt="Company Logo" />
        </div>
        <p class="bold-heading">
          Welcome, Pulkit Aggarwal 🙌
          <br />
          Our mission is to make you
          <br />
          more productive. This will only take a minute.
          <br />
        </p>
        <main-button @click="goto('div1')" content="Let's do it!"></main-button>
      </div>

      <div class="step-1 bot" ref="div1">
        <div class="logo-main">
          <img src="./assets/logo-click.png" alt="Company Logo" />
        </div>
        <p class="bold-heading">
          Name your Workspace:
        </p>
        <br />
        <div class="input-container">
          <input type="text" class="step-1-input" />
        </div>
        <div class="enter">
          Press enter
        </div>
        <main-button @click="goto('div2')" content="Next"></main-button>
      </div>

      <div class="step-2 bot" ref="div2">
        <div class="logo-main">
          <img src="./assets/logo-click.png" alt="Company Logo" />
        </div>
        <p class="bold-heading">
          Customize your Workspace's avatar:
        </p>
        <br />
        <div class="avatar">
          <div class="image-drop">
            <div class="drop">Drop an image here</div>
          </div>
          <div class="sep">
            <span>Or</span>
          </div>

          <div class="name-avatar">
            P
          </div>
        </div>

        <div class="radio-buttons-theme">
          <Circle class="inline" style="background:#705eeb"></Circle>
          <Circle class="inline" style="background:blue "></Circle>
          <Circle class="inline" style="background:green "></Circle>
          <Circle class="inline" style="background:#705e "></Circle>
          <Circle class="inline" style="background:#7eeb "></Circle>
          <Circle class="inline" style="background:#765e "></Circle>
          <Circle class="inline" style="background:#755e "></Circle>
          <Circle class="inline" style="background:#301 "></Circle>
          <Circle class="inline" style="background:black"></Circle>
        </div>
        <main-button
          @click="goto('div3')"
          content="I'm happy so far"
        ></main-button>
      </div>

      <div class="step-3 bot" ref="div3">
        <div class="logo-main">
          <img src="./assets/logo-click.png" alt="Company Logo" />
        </div>
        <p class="bold-heading">
          Choose your favorite color theme:
        </p>
        <br />
        <div class="radio-buttons-theme">
          <Circle class="inline" style="background:#705eeb"></Circle>
          <Circle class="inline" style="background:blue "></Circle>
          <Circle class="inline" style="background:green "></Circle>
          <Circle class="inline" style="background:#705e "></Circle>
          <Circle class="inline" style="background:#7eeb "></Circle>
          <Circle class="inline" style="background:#765e "></Circle>
          <Circle class="inline" style="background:#755e "></Circle>
          <Circle class="inline" style="background:#301 "></Circle>
          <Circle class="inline" style="background:black"></Circle>
        </div>
        <main-button
          @click="goto('div4')"
          content="I'm Happy so far"
        ></main-button>
      </div>

      <div class="step-4 bot" ref="div4">
        <div class="logo-main">
          <img src="./assets/logo-click.png" alt="Company Logo" />
        </div>
        <p class="bold-heading">
          How many people will you be working with?
        </p>
        <br />
        <div class="choices">
          <box @click="goto('div5')" title="Just me"></box>
          <box @click="goto('div5')" title="6-10"></box>
          <box @click="goto('div5')" title="11-25"></box>
          <box @click="goto('div5')" title="26-50"></box>
          <box @click="goto('div5')" title="51-200"></box>
          <box @click="goto('div5')" title="201-500"></box>
          <box @click="goto('div5')" title="501+"></box>
          <box @click="goto('div5')" title="I don't know"></box>
        </div>
      </div>

      <div class="step-5 bot" ref="div5">
        <div class="logo-main">
          <img src="./assets/logo-click.png" alt="Company Logo" />
        </div>
        <p class="bold-heading">
          What are you trying to accomplish using ClickUp?
        </p>
        <br />

        <div class="choices">
          <box title="Remote onboarding"></box>
          <box title="Project management"></box>
          <box title="To-do's & Lists"></box>
          <box title="Sales & CRM"></box>
          <box title="Finance management"></box>
          <box title="Campaign management"></box>
          <box title="Sprints & backlogs"></box>
          <box title="Getting things done"></box>
          <box title="Remote work management"></box>
          <box title="Event planningt"></box>
          <box title="Save time"></box>
          <box title="Replace multiple apps with one"></box>
          <box title="Personal"></box>
          <box title="Other"></box>
          <box title="I don't know"></box>
        </div>
        <main-button @click="goto('div6')" content="Next"></main-button>
        <div class="text">Friendly note: You can select multiple options.</div>
      </div>

      <div class="step-6 bot" ref="div6">
        <div class="logo-main">
          <img src="./assets/logo-click.png" alt="Company Logo" />
        </div>
        <p class="bold-heading">
          How did you hear about us?
        </p>
        <br />

        <div class="choices">
          <box
            @click="goto('div5')"
            title="Search Engine (Google, Bing, etc.)"
          ></box>
          <box @click="goto('div7')" title="Google Ads"></box>
          <box @click="goto('div7')" title="Facebook Ads"></box>
          <box @click="goto('div7')" title="Youtube Ads"></box>
          <box @click="goto('div7')" title="Social Media"></box>
          <box @click="goto('div7')" title="Email"></box>
          <box @click="goto('div7')" title="Audio/Podcasts"></box>
          <box @click="goto('div7')" title="TV"></box>
          <box @click="goto('div7')" title="Newspaper"></box>
          <box @click="goto('div7')" title="Billboard"></box>
          <box @click="goto('div7')" title="Word of Mouth"></box>
          <box @click="goto('div7')" title="Other"></box>
        </div>
        <main-button @click="goto('div7')" content="Next"></main-button>
      </div>

      <div class="step-7 bot" ref="div7">
        <div class="logo-main">
          <img src="./assets/logo-click.png" alt="Company Logo" />
        </div>
        <p class="bold-heading">
          Invite people to your Workspace:
        </p>
        <br />
        <div class="input-container">
          <input
            type="text"
            placeholder="Enter email addresses (or paste multiple)"
          />
        </div>
        <div class="enter">
          Press enter
        </div>
        <main-button @click="goto('div8')" content="I'm done"></main-button>
      </div>

      <div class="step-8 bot" ref="div8">
        <div class="logo-main">
          <img src="./assets/logo-click.png" alt="Company Logo" />
        </div>
        <p class="bold-heading">
          Customize how you work by enabling ClickApps
        </p>
        <br />
        <div class="choices">
          <box title="Remote onboarding"></box>
          <box title="Project management"></box>
          <box title="To-do's & Lists"></box>
          <box title="Sales & CRM"></box>
          <box title="Finance management"></box>
          <box title="Campaign management"></box>
          <box title="Sprints & backlogs"></box>
          <box title="Getting things done"></box>
          <box title="Remote work management"></box>
          <box title="Event planningt"></box>
          <box title="Save time"></box>
          <box title="Replace multiple apps with one"></box>
          <box title="Personal"></box>
          <box title="Other"></box>
          <box title="I don't know"></box>
        </div>
        <main-button @click="goto('div9')" content="Looks good"></main-button>
        <div class="text">Friendly note: You can adjust ClickApps anytime.</div>
      </div>

      <div class="step-9 bot" ref="div9">
        <div class="logo-main">
          <img src="./assets/logo-click.png" alt="Company Logo" />
        </div>
        <p class="bold-heading">
          Do you use any of these apps?
        </p>
        <br />
        <div class="choices">
          <!-- <i class="fab fa-slack">Slack</i> -->
          <box title="Slack"> </box>
          <box title="Zapier"></box>
          <box title="Microsoft Teams"></box>
          <box title="Zoom"></box>
          <box title="Github"></box>
          <box title="Gitlab"></box>
          <box title="Bitbucket"></box>
          <box title="Hangouts"></box>
          <box title="Zendesk"></box>
        </div>
        <main-button @click="goto('div10')" content="I'm done"></main-button>
      </div>

      <div class="step-10 bot" ref="div10">
        <div class="logo-main">
          <img src="./assets/logo-click.png" alt="Company Logo" />
        </div>
        <p class="bold-heading">
          Do you want to import tasks?
        </p>
        <br />
        <div class="choices">
          <!-- <i class="fab fa-slack">Slack</i> -->
          <box title="Asana"> </box>
          <box title="Basecamp"></box>
          <box title="Trello"></box>
          <box title="Jira"></box>
          <box title="Wrike"></box>
          <box title="To do list"></box>
          <box title="Monday"></box>
        </div>
        <main-button @click="goto('div11')" content="I'm done"></main-button>
      </div>

      <div class="step-11 bot" ref="div11">
        <div class="logo-main">
          <img src="./assets/logo-click.png" alt="Company Logo" />
        </div>
        <p class="bold-heading">
          That's it. Now go and change the world!
          <br />
          And don't forget to have fun 🙌
        </p>
        <br />
        <main-button content="Play with ClickUp"></main-button>
      </div>
    </div>

    <div class="side"></div>
  </div>
</template>

<script>
import MainButton from "./components/MainButton";
import Box from "./components/Box.vue";
import Circle from "./components/Circle";
export default {
  name: "App",
  components: { MainButton, Box, Circle },
  methods: {
    goto(refName) {
      var element = this.$refs[refName];
      var top = element.offsetTop;
      window.scrollTo(0, top);
    },
  },
};
</script>

<style>
@import url("https://fonts.googleapis.com/css2?family=Comfortaa:wght@400;500;600;700&display=swap");
* {
  padding: 0;
  margin: 0;
  box-sizing: border-box;
  font-family: "Comfortaa", cursive;
}

#app {
  background-color: #fff;
  color: #000;
}

.bot {
  margin-bottom: 130px;
}

.welcome {
  display: grid;
  grid-template-columns: 1fr 20%;
  grid-template-rows: 1fr;
  grid-template-areas: "main side";
  height: 100%;
  width: 100%;
}

.main {
  grid-area: main;
  margin-left: 15vw;
  margin-right: 5vw;
}

.side {
  grid-area: side;
  background-color: #705eeb;
}
/* Start */

.start {
  padding-top: 48vh;
}
.bold-heading {
  margin-top: 10vh;
  font-size: 1.35em;
  line-height: 1.4em;
  padding: 15px;
  padding-left: 0;
}
img {
  height: 9vh;
  float: left;
  margin-left: -7vw;
  margin-top: 10px;
}

/* Start section end */

/* Step -1 */
.input-container input {
  background-color: transparent;
  box-shadow: none;
  width: 100%;
  display: block;
  border: 0;
  outline: none;
  font-size: 2em;
  font-weight: 300;
  font-family: "Comfortaa", cursive !important;
}

.input-container {
  border-bottom: 1px solid #705eeb;
}

.enter {
  text-align: right;
  margin-top: 10px;
  font-size: 14px;
  display: flex;
  align-items: center;
  justify-content: flex-end;
  height: 50px;
  color: #705eeb;
}

/* Step-1 end */

/* Step-2 start */
.avatar {
  display: flex;
  position: relative;
  margin-bottom: 30px;
}

.image-drop {
  width: 140px;
  height: 140px;
  border: 1px dashed #705eeb;
  border-radius: 140px;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  /* position: relative; */
}

.drop {
  font-size: 12px;
  text-align: center;
  margin-top: 10px;
  line-height: 20px;
}

.sep {
  display: flex;
  flex-direction: column;
  align-items: center;
  margin-left: 30px;
  margin-right: 30px;
  justify-content: center;
  opacity: 0.4;
}

.name-avatar {
  width: 140px;
  height: 140px;
  border-radius: 140px;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  background-color: #705eeb;
  color: #fff;
  font-size: 3em;
}

.radio-buttons-workspace {
  display: flex;
  align-items: center;
  flex-wrap: wrap;
  width: 31vw;
  padding-left: 50px;
  justify-content: center;
}

.items-workspace {
  display: flex;
  justify-content: center;
  align-items: center;
  flex-wrap: wrap;
  padding: 10px;
}

/* Step -2 end */

/* Step -3 start*/

.inline {
  display: inline-flex !important;
}

/* step3 end */

/* Step-4 start */
.choices {
  display: flex;
  flex-wrap: wrap;
  margin-bottom: 30px;
}
/* Step -4 end */

/* Step -5 start */

.text {
  display: inline-block;
  padding-left: 10px;
  font-size: 10px;
  color: rgb(206, 201, 201);
}

/* Step-5 end */

/* blur start */
/* #app *:not(.active) {
  filter: blur(3px);
} */
/* Blur end */

@media (max-width: 768px) {
  .welcome {
    display: block;
    border: none;
    overflow: hidden;
    min-width: 100%;
    max-width: 100%;
  }
  .name-avatar {
    width: 105px;
    height: 105px;
  }
  .image-drop {
    width: 105px;
    height: 105px;
  }
}
</style>
