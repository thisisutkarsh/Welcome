<template>
  <div class="welcome">
    <div class="main">
      <div class="start">
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
        <main-button content="Let's do it!"></main-button>
      </div>

      <div class="step-1">
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
        <main-button content="Next"></main-button>
      </div>

      <div class="step-2">
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

        <div class="radio-buttons-workspace"></div>
        <main-button content="I'm happy so far"></main-button>
      </div>

      <div class="step-3">
        <div class="logo-main">
          <img src="./assets/logo-click.png" alt="Company Logo" />
        </div>
        <p class="bold-heading">
          Choose your favorite color theme:
        </p>
        <br />
        <div class="radio-buttons-theme"></div>
        <main-button content="I'm Happy so far"></main-button>
      </div>

      <div class="step-4">
        <div class="logo-main">
          <img src="./assets/logo-click.png" alt="Company Logo" />
        </div>
        <p class="bold-heading">
          How many people will you be working with?
        </p>
        <br />
        <div class="choices">
          <box title="Just me"></box>
          <box title="6-10"></box>
          <box title="11-25"></box>
          <box title="26-50"></box>
          <box title="51-200"></box>
          <box title="201-500"></box>
          <box title="501+"></box>
          <box title="I don't know"></box>
        </div>
      </div>

      <div class="step-5">
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
        <main-button content="Next"></main-button>
        <div class="text">Friendly note: You can select multiple options.</div>
      </div>
    </div>

    <div class="side"></div>
  </div>
</template>

<script>
import MainButton from "./components/MainButton";
import Box from "./components/Box.vue";
export default {
  name: "App",
  components: { MainButton, Box },
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

.welcome {
  display: grid;
  grid-template-columns: 1fr 400px;
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
  margin-bottom: 10px;
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
/* Step -2 end */

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
</style>
