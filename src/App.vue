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
          title: "Both",
          type: "normal",
          handler: () => {
            this.nextQuestion();
          },
        },
      ],
      {
        defaultAction: 2,
      }
    );
    // this.nextQuestion();
  },
  methods: {
    random(max) {
      return Math.floor(Math.random() * max);
    },
    getChoices(isIon, aspect) {
      if (isIon) {
        let res = [];
        for (var ionIndex in this.ions) {
          var ion = this.ions[ionIndex];
          // console.log(ion[aspect])
          if (ion[aspect] != undefined && res.includes(ion[aspect]) == false) {
            // console.log(ion[aspect])
            res.push(ion[aspect]);
          }
        }
        console.log(res);
        return res;
      } else {
        let res = [];
        for (var index in this.compounds) {
          var compound = this.compounds[index];
          // console.log(ion[aspect])
          if (
            compound[aspect] != undefined &&
            res.includes(String(compound[aspect])) == false
          ) {
            // console.log(ion[aspect])
            res.push(String(compound[aspect]));
          }
        }
        console.log(res);
        return res;
      }
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
    nextQuestion() {
      var question, answer, choices, actions, x;
      let mode = this.random(2);
      if (this.preferredMode == "ions") {
        mode = 0;
      } else if (this.preferredMode == "compounds") {
        mode = 1;
      }
      if (mode == 0) {
        // Ions
        let obj = this.ions[this.random(this.ions.length)];
        let aspects = ["solution", "flame"];
        let aspect = aspects[this.random(2)];
        switch (aspect) {
          case "solution":
            question = "What is the colour of a " + obj.name + " solution?";
            answer = obj.solution;
            choices = this.shuffle(this.getChoices(true, aspect));
            actions = [];
            for (x in choices) {
              let choice = choices[x];
              if (choice != answer) {
                actions.push({
                  title: choice,
                  type: "normal",
                  handler: () => {
                    this.$alert.present(
                      "Incorrect",
                      "The colour of a " + obj.name + " solution is " + answer,
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
                      "The colour of a " + obj.name + " solution is " + answer,
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
            this.$alert.present("Question", question, actions);
            break;
          case "flame":
            question =
              "What colour would be observed in a flame test for " +
              obj.name +
              "?";
            answer = obj.flame;
            choices = this.shuffle(this.getChoices(true, aspect));
            actions = [];
            for (x in choices) {
              let choice = choices[x];
              if (choice != answer) {
                actions.push({
                  title: choice,
                  type: "normal",
                  handler: () => {
                    this.$alert.present(
                      "Incorrect",
                      "The colour of the flame of " +
                        obj.name +
                        " should be " +
                        answer,
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
                      "The colour of the flame of " +
                        obj.name +
                        " solution is " +
                        answer,
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
            this.$alert.present("Question", question, actions);
            break;
        }
      } else {
        // Compounds
        let obj = this.compounds[this.random(this.compounds.length)];
        let aspects = ["soluble", "colour"];
        // console.log(aspects);
        // console.log(aspects);
        let aspect = aspects[this.random(aspects.length)];
        console.log(aspect);
        // console.log(aspect);
        switch (aspect) {
          case "soluble":
            question = obj.name + " is soluble.";
            answer = String(obj.soluble);
            choices = this.shuffle(this.getChoices(false, aspect));
            actions = [];
            for (x in choices) {
              let choice = choices[x];
              if (choice != answer) {
                actions.push({
                  title: choice,
                  type: "normal",
                  handler: () => {
                    this.$alert.present(
                      "Incorrect",
                      "The answer is " + answer,
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
                      "The answer is " + answer,
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
            this.$alert.present("Question", question, actions);
            break;
          case "colour":
            question =
              "What is the colour of " + obj.name + " precipitate, if any?";
            answer = obj.colour;
            choices = this.shuffle(this.getChoices(false, aspect));
            actions = [];
            for (x in choices) {
              let choice = choices[x];
              if (choice != answer) {
                actions.push({
                  title: choice,
                  type: "normal",
                  handler: () => {
                    this.$alert.present(
                      "Incorrect",
                      "The colour of " + obj.name + " should be: " + answer,
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
                      "The colour of " + obj.name + " is " + answer,
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
            this.$alert.present("Question", question, actions);
            break;
        }
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
