<template>
  <div id="app">
    <alert></alert>
  </div>
</template>

<script>
export default {
  name: "App",
  components: {},
  data: () => ({
    preferredMode: null,
    compounds: [
      {
        name: "Barium Phosphate",
        soluble: "No",
        colour: "White",
      },
      {
        name: "Barium Sulfate",
        soluble: "No",
        colour: "White",
      },
      {
        name: "Barium Carbonate",
        soluble: "No",
        colour: "White",
      },
      {
        name: "Barium Hydroxide",
        soluble: "Slightly", // Slightly soluble
        colour: "White",
        info: "Slightly soluble",
      },
      {
        name: "Barium Chloride",
        soluble: "Yes",
        colour: "No precipitate",
      },
      {
        name: "Barium Bromide",
        soluble: "Yes",
        colour: "No precipitate",
      },
      {
        name: "Barium Iodide",
        soluble: "Yes",
        colour: "No precipitate",
      },
      {
        name: "Barium Acetate",
        soluble: "Yes",
        colour: "No precipitate",
      },
      {
        name: "Calcium Phosphate",
        soluble: "No",
        colour: "White",
      },
      {
        name: "Calcium Sulfate",
        soluble: "Slightly", // Slightly
        colour: "White",
        info: "Slightly soluble",
      },
      {
        name: "Calcium Carbonate",
        soluble: "No",
        colour: "White",
      },
      {
        name: "Calcium Hydroxide",
        soluble: "Slightly", // Slightly
        colour: "White",
        info: "Slightly soluble",
      },
      {
        name: "Calcium Chloride",
        soluble: "Yes",
        colour: "No precipitate",
      },
      {
        name: "Calcium Bromide",
        soluble: "Yes",
        colour: "No precipitate",
      },
      {
        name: "Calcium Iodide",
        soluble: "Yes",
        colour: "No precipitate",
      },
      {
        name: "Calcium Acetate",
        soluble: "Yes",
        colour: "No precipitate",
      },
      {
        name: "Magnesium Phosphate",
        soluble: "No",
        colour: "White",
      },
      {
        name: "Magnesium Sulfate",
        soluble: "Yes",
        colour: "No precipitate",
      },
      {
        name: "Magnesium Carbonate",
        soluble: "No",
        colour: "White",
      },
      {
        name: "Magnesium Hydroxide",
        soluble: "No",
        colour: "White",
      },
      {
        name: "Magnesium Chloride",
        soluble: "Yes",
        colour: "No precipitate",
      },
      {
        name: "Magnesium Bromide",
        soluble: "Yes",
        colour: "No precipitate",
      },
      {
        name: "Magnesium Iodide",
        soluble: "Yes",
        colour: "No precipitate",
      },
      {
        name: "Magnesium Acetate",
        soluble: "Yes",
        colour: "No precipitate",
      },
      {
        name: "Lead (II) Phosphate",
        soluble: "No",
        colour: "White",
      },
      {
        name: "Lead (II) Sulfate",
        soluble: "No",
        colour: "White",
      },
      {
        name: "Lead (II) Carbonate",
        soluble: "No",
        colour: "White",
      },
      {
        name: "Lead (II) Hydroxide",
        soluble: "No",
        colour: "White",
      },
      {
        name: "Lead (II) Chloride",
        soluble: "Slightly",
        colour: "White",
        info: "Slightly soluble",
      },
      {
        name: "Lead (II) Bromide",
        soluble: "Slightly",
        colour: "White",
        info: "Slightly soluble",
      },
      {
        name: "Lead (II) Iodide",
        soluble: "No",
        colour: "Yellow",
      },
      {
        name: "Lead (II) Acetate",
        soluble: "Yes",
        colour: "No precipitate",
      },
      {
        name: "Copper (II) Phosphate",
        soluble: "No",
        colour: "Blue",
      },
      {
        name: "Copper (II) Sulfate",
        soluble: "Yes",
        // colour: "Blue",
        colour: "No precipitate",
      },
      {
        name: "Copper (II) Carbonate",
        soluble: "No",
        colour: "Green",
      },
      {
        name: "Copper (II) Hydroxide",
        soluble: "No",
        colour: "Blue",
      },
      {
        name: "Copper (II) Chloride",
        soluble: "Yes",
        // colour: "Blue",
        colour: "No precipitate",
      },
      {
        name: "Copper (II) Bromide",
        soluble: "Yes",
        // colour: "Blue",
        colour: "No precipitate",
      },
      {
        name: "Copper (II) Iodide",
        soluble: "Unstable",
        colour: "Unstable",
      },
      {
        name: "Copper (II) Acetate",
        soluble: "Yes",
        // colour: "Blue",
        colour: "No precipitate",
      },
      {
        name: "Iron (II) Phosphate",
        soluble: "No",
        colour: "Green",
      },
      {
        name: "Iron (II) Sulfate",
        soluble: "Yes",
        // colour: "Green",
        colour: "No precipitate",
      },
      {
        name: "Iron (II) Carbonate",
        soluble: "No",
        colour: "Grey",
      },
      {
        name: "Iron (II) Hydroxide",
        soluble: "No",
        colour: "Green",
      },
      {
        name: "Iron (II) Chloride",
        soluble: "Yes",
        // colour: "Green",
        colour: "No precipitate",
      },
      {
        name: "Iron (II) Bromide",
        soluble: "Yes",
        // colour: "Green",
        colour: "No precipitate",
      },
      {
        name: "Iron (II) Iodide",
        soluble: "Yes",
        // colour: "Green",
        colour: "No precipitate",
      },
      {
        name: "Iron (II) Acetate",
        soluble: "Yes",
        // colour: "Green",
        colour: "No precipitate",
      },
      {
        name: "Iron (III) Phosphate",
        soluble: "No",
        colour: "Yellow",
      },
      {
        name: "Iron (III) Sulfate",
        soluble: "Yes",
        // colour: "Yellow",
        colour: "No precipitate",
      },
      {
        name: "Iron (III) Carbonate",
        soluble: "Unstable",
        colour: "Unstable",
      },
      {
        name: "Iron (III) Hydroxide",
        soluble: "No",
        colour: "Brown",
      },
      {
        name: "Iron (III) Chloride",
        soluble: "Yes",
        // colour: "Brown",
        colour: "No precipitate",
      },
      {
        name: "Iron (III) Bromide",
        soluble: "Yes",
        // colour: "Brown",
        colour: "No precipitate",
      },
      {
        name: "Iron (III) Iodide",
        soluble: "Unstable",
        colour: "Unstable",
      },
      {
        name: "Iron (III) Acetate",
        soluble: "Slightly",
        colour: "Brown",
        info: "Slightly soluble",
      },
      {
        name: "Silver Phosphate",
        soluble: "No",
        colour: "Yellow",
      },
      {
        name: "Silver Sulfate",
        soluble: "Slightly",
        colour: "White",
        info: "Slightly soluble",
      },
      {
        name: "Silver Carbonate",
        soluble: "No",
        colour: "Yellow",
      },
      {
        name: "Silver Chloride",
        soluble: "No",
        colour: "White",
      },
      {
        name: "Silver Bromide",
        soluble: "No",
        colour: "Yellow",
      },
      {
        name: "Silver Iodide",
        soluble: "No",
        colour: "Yellow",
      },
      {
        name: "Silver Acetate",
        soluble: "Slightly",
        colour: "White",
        info: "Slightly soluble",
      },
    ],
    ions: [
      {
        name: "Barium",
        solution: "Colourless",
        flame: "Apple Green",
      },
      {
        name: "Calcium",
        solution: "Colourless",
        flame: "Brick Red",
      },
      {
        name: "Magnesium",
        solution: "Colourless",
        flame: "No characteristic flame colour",
      },
      {
        name: "Lead (II)",
        solution: "Colourless",
        flame: "Gray-White",
      },
      {
        name: "Copper (II)",
        solution: "Blue",
        flame: "Blue-Green",
      },
      {
        name: "Iron (II)",
        solution: "Pale Green",
        flame: "Orange-Brown",
      },
      {
        name: "Iron (III)",
        solution: "Yellow",
        flame: "Orange-Brown",
      },
      {
        name: "Silver",
        solution: "Colourless",
        flame: "No characteristic flame colour",
      },
    ],
    cations: [
      {
        name: "Lead (II)",
        hcl: "White precipitate",
        h2so4: "No reaction",
        naoh: "No reaction",
      },
      {
        name: "Silver",
        hcl: "White precipitate",
        h2so4: "No reaction",
        naoh: "No reaction",
      },
      {
        name: "Barium",
        hcl: "No reaction",
        h2so4: "White precipitate",
        naoh: "No reaction",
      },
      {
        name: "Calcium",
        hcl: "No reaction",
        h2so4: "White precipitate",
        naoh: "No reaction",
      },
      {
        name: "Magnesium (II)",
        hcl: "No reaction",
        h2so4: "No reaction",
        naoh: "No reaction",
      },
      {
        name: "Copper (II)",
        hcl: "No reaction",
        h2so4: "No reaction",
        naoh: "Pale-blue precipitate",
      },
      {
        name: "Iron (II)",
        hcl: "No reaction",
        h2so4: "No reaction",
        naoh: "Green precipitate",
      },
      {
        name: "Iron (III)",
        hcl: "No reaction",
        h2so4: "No reaction",
        naoh: "Brown precipitate",
      },
    ],
    anions: [
      {
        name: "Carbonate",
        ph: ">7",
      },
      {
        name: "Acetate",
        ph: ">7",
      },
      {
        name: "Hydroxide",
        ph: ">7",
      },
      {
        name: "Phosphate",
        ph: ">7",
      },
      {
        name: "Sulfate",
        ph: "=7",
      },
      {
        name: "Chloride",
        ph: "=7",
      },
      {
        name: "Bromide",
        ph: "=7",
      },
      {
        name: "Iodide",
        ph: "=7",
      },
      // [TODO] add more reactions
    ],
  }),
  mounted() {
    this.$alert.present(
      "Mode selection",
      "Which questions should be in the quiz?",
      [
        {
          title: "Flame Tests & Solution Colours",
          type: "normal",
          handler: () => {
            this.preferredMode = "ions";
            this.nextQuestion();
          },
        },
        {
          title: "Solubility & Precipitate Colours",
          type: "normal",
          handler: () => {
            this.preferredMode = "compounds";
            this.nextQuestion();
          },
        },
        {
          title: "Cation Reactions & Identification",
          type: "normal",
          handler: () => {
            this.preferredMode = "cations";
            this.nextQuestion();
          },
        },
        {
          // title: "Anion Reactions & Identification",
          title: "Anion pH",
          type: "normal",
          handler: () => {
            this.preferredMode = "anions";
            this.nextQuestion();
          },
        },
        {
          title: "All",
          type: "normal",
          handler: () => {
            this.nextQuestion();
          },
        },
      ],
      {
        defaultAction: 4,
      }
    );
    // this.nextQuestion();
  },
  methods: {
    random(max) {
      return Math.floor(Math.random() * max);
    },
    getChoices(array, aspect) {
      let res = [];
      for (var index in array) {
        var obj = array[index];
        if (obj[aspect] != undefined && res.includes(obj[aspect]) == false) {
          res.push(obj[aspect]);
        }
      }
      return res;
    },
    shuffle(array) {
      let currentIndex = array.length,
        randomIndex;

      // While there remain elements to shuffle...
      while (currentIndex != 0) {
        // Pick a remaining element...
        randomIndex = Math.floor(Math.random() * currentIndex);
        currentIndex--;

        // And swap it with the current element.
        [array[currentIndex], array[randomIndex]] = [
          array[randomIndex],
          array[currentIndex],
        ];
      }
      return array;
    },
    showQuestion(question, choices, answer, correctmessage, incorrectmessage) {
      var x;
      var actions = [];
      for (x in choices) {
        let choice = choices[x];
        if (choice != answer) {
          actions.push({
            title: choice,
            type: "normal",
            handler: () => {
              this.$alert.present(
                "Incorrect",
                incorrectmessage,
                [
                  {
                    title: "Next Question",
                    type: "normal",
                    handler: () => {
                      this.nextQuestion();
                    },
                  },
                ],
                {
                  defaultAction: 0,
                  defaultEscapeAction: 0,
                }
              );
            },
          });
        } else {
          actions.push({
            title: choice,
            type: "normal",
            handler: () => {
              this.$alert.present(
                "Correct",
                correctmessage,
                [
                  {
                    title: "Next Question",
                    type: "normal",
                    handler: () => {
                      this.nextQuestion();
                    },
                  },
                ],
                {
                  defaultAction: 0,
                  defaultEscapeAction: 0,
                }
              );
            },
          });
        }
      }
      actions.push({
        title: "Skip",
        type: "destructive",
        handler: () => {
          this.nextQuestion();
        },
      });
      this.$alert.present("Question", question, actions, {
        defaultEscapeAction: actions.length - 1,
      });
    },
    nextQuestion() {
      var question, answer, choices, obj, aspects, aspect;
      var modes = ["ions", "compounds", "cations", "anions"];
      let mode = modes[this.random(4)];
      if (this.preferredMode != null) {
        mode = this.preferredMode;
      }
      switch (mode) {
        case "ions":
          // Ions
          obj = this.ions[this.random(this.ions.length)];
          aspects = ["solution", "flame"];
          aspect = aspects[this.random(2)];
          switch (aspect) {
            case "solution":
              question = "What is the colour of a " + obj.name + " solution?";
              answer = obj.solution;
              choices = this.shuffle(this.getChoices(this.ions, aspect));
              this.showQuestion(
                question,
                choices,
                answer,
                "That's correct. " +
                  obj.name +
                  " is " +
                  answer +
                  " in solution",
                "That's wrong. " + obj.name + " is " + answer + " in solution"
              );
              break;
            case "flame":
              question =
                "What colour would be observed in a flame test for " +
                obj.name +
                "?";
              answer = obj.flame;
              choices = this.shuffle(this.getChoices(this.ions, aspect));
              this.showQuestion(
                question,
                choices,
                answer,
                "That's correct, the colour of the flame should be " + answer,
                "No, the colour of the flame for " +
                  obj.name +
                  " should be " +
                  answer
              );
              break;
          }
          break;
        case "compounds":
          obj = this.compounds[this.random(this.compounds.length)];
          aspects = ["soluble", "colour"];
          aspect = aspects[this.random(aspects.length)];
          switch (aspect) {
            case "soluble":
              question = obj.name + " is soluble.";
              answer = String(obj.soluble);
              choices = this.shuffle(this.getChoices(this.compounds, aspect));
              this.showQuestion(
                question,
                choices,
                answer,
                "Correct. The answer is " + answer,
                "No, it should be " + answer
              );
              break;
            case "colour":
              question =
                "What is the colour of " + obj.name + " if it precipitates?";
              answer = obj.colour;
              choices = this.shuffle(this.getChoices(this.compounds, aspect));
              this.showQuestion(
                question,
                choices,
                answer,
                "Correct. The colour of " + obj.name + " is " + answer,
                "No, it should be " + answer
              );
              break;
          }
          break;
        case "cations":
          obj = this.cations[this.random(this.cations.length)];
          aspects = ["hcl", "h2so4", "naoh"];
          aspect = aspects[this.random(aspects.length)];
          switch (aspect) {
            case "hcl":
              question =
                "Outline the expected observation if " +
                obj.name +
                " is reacted with hydrochloric acid.";
              answer = obj.hcl;
              choices = this.shuffle(this.getChoices(this.cations, aspect));
              this.showQuestion(
                question,
                choices,
                answer,
                "Correct. " + answer,
                "No, we should expect " + answer
              );
              break;
            case "h2so4":
              question =
                "Outline the expected observation if " +
                obj.name +
                " is reacted with sulfuric acid.";
              answer = obj.h2so4;
              choices = this.shuffle(this.getChoices(this.cations, aspect));
              this.showQuestion(
                question,
                choices,
                answer,
                "Correct. " + answer,
                "No, we should expect " + answer
              );
              break;
            case "naoh":
              question =
                "Outline the expected observation if " +
                obj.name +
                " is reacted with sodium hydroxide.";
              answer = obj.naoh;
              choices = this.shuffle(this.getChoices(this.cations, aspect));
              this.showQuestion(
                question,
                choices,
                answer,
                "Correct. " + answer,
                "No, we should expect " + answer
              );
              break;
          }
          break;
        case "anions":
          obj = this.anions[this.random(this.anions.length)];
          // aspects = ["ph", "hno3", "feno33", "bano32", "agno3"]; // TODO
          aspects = ["ph"];
          aspect = aspects[this.random(aspects.length)];
          switch (aspect) {
            case "ph":
              question = "What is the pH for " + obj.name + "?";
              answer = obj.ph;
              choices = this.shuffle(this.getChoices(this.anions, aspect));
              this.showQuestion(
                question,
                choices,
                answer,
                "Correct. pH" + answer,
                "No, we should expect pH" + answer
              );
              break;
          }
          break;
      }
    },
  },
};
</script>

<style>
@import url("https://fonts.googleapis.com/css2?family=Inter:wght@100;200;300;400;500;600;700;800;900&display=swap");
body {
  font-family: "Inter", sans-serif;
}
</style>
