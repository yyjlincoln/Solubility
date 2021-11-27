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
    compounds: [
      {
        name: "Barium Phosphate",
        soluable: false,
        colour: "White",
      },
      {
        name: "Barium Sulfate",
        soluable: false,
        colour: "White",
      },
      {
        name: "Barium Carbonate",
        soluable: false,
        colour: "White",
      },
      {
        name: "Barium Hydroxide",
        soluable: false, // Slightly soluable
        colour: "White",
        info: "Slightly soluable",
      },
      {
        name: "Barium Chloride",
        soluable: true,
        colour: "No precipitate",
      },
      {
        name: "Barium Bromide",
        soluable: true,
        colour: "No precipitate",
      },
      {
        name: "Barium Iodide",
        soluable: true,
        colour: "No precipitate",
      },
      {
        name: "Barium Acetate",
        soluable: true,
        colour: "No precipitate",
      },
      {
        name: "Calcium Phosphate",
        soluable: false,
        colour: "White",
      },
      {
        name: "Calcium Sulfate",
        soluable: false, // Slightly
        colour: "White",
        info: "Slightly soluable",
      },
      {
        name: "Calcium Carbonate",
        soluable: false,
        colour: "White",
      },
      {
        name: "Calcium Hydroxide",
        soluable: false, // Slightly
        colour: "White",
        info: "Slightly soluable",
      },
      {
        name: "Calcium Chloride",
        soluable: true,
        colour: "No precipitate",
      },
      {
        name: "Calcium Bromide",
        soluable: true,
        colour: "No precipitate",
      },
      {
        name: "Calcium Iodide",
        soluable: true,
        colour: "No precipitate",
      },
      {
        name: "Calcium Acetate",
        soluable: true,
        colour: "No precipitate",
      },
      {
        name: "Magnesium Phosphate",
        soluable: false,
        colour: "White",
      },
      {
        name: "Magnesium Sulfate",
        soluable: true,
        colour: "No precipitate",
      },
      {
        name: "Magnesium Carbonate",
        soluable: false,
        colour: "White",
      },
      {
        name: "Magnesium Hydroxide",
        soluable: false,
        colour: "White",
      },
      {
        name: "Magnesium Chloride",
        soluable: true,
        colour: "No precipitate",
      },
      {
        name: "Magnesium Bromide",
        soluable: true,
        colour: "No precipitate",
      },
      {
        name: "Magnesium Iodide",
        soluable: true,
        colour: "No precipitate",
      },
      {
        name: "Magnesium Acetate",
        soluable: true,
        colour: "No precipitate",
      },
      {
        name: "Lead (II) Phosphate",
        soluable: false,
        colour: "White",
      },
      {
        name: "Lead (II) Sulfate",
        soluable: false,
        colour: "White",
      },
      {
        name: "Lead (II) Carbonate",
        soluable: false,
        colour: "White",
      },
      {
        name: "Lead (II) Hydroxide",
        soluable: false,
        colour: "White",
      },
      {
        name: "Lead (II) Chloride",
        soluable: false,
        colour: "White",
        info: "Slightly soluable",
      },
      {
        name: "Lead (II) Bromide",
        soluable: false,
        colour: "White",
        info: "Slightly soluable",
      },
      {
        name: "Lead (II) Iodide",
        soluable: false,
        colour: "Yellow",
      },
      {
        name: "Lead (II) Acetate",
        soluable: true,
        colour: "No precipitate",
      },
      {
        name: "Copper (II) Phosphate",
        soluable: false,
        colour: "Blue",
      },
      {
        name: "Copper (II) Sulfate",
        soluable: true,
        // colour: "Blue",
        colour: "No precipitate",
      },
      {
        name: "Copper (II) Carbonate",
        soluable: false,
        colour: "Green",
      },
      {
        name: "Copper (II) Hydroxide",
        soluable: false,
        colour: "Blue",
      },
      {
        name: "Copper (II) Chloride",
        soluable: true,
        // colour: "Blue",
        colour: "No precipitate",
      },
      {
        name: "Copper (II) Bromide",
        soluable: true,
        // colour: "Blue",
        colour: "No precipitate",
      },
      {
        name: "Copper (II) Acetate",
        soluable: true,
        // colour: "Blue",
        colour: "No precipitate",
      },
      {
        name: "Iron (II) Phosphate",
        soluable: false,
        colour: "Green",
      },
      {
        name: "Iron (II) Sulfate",
        soluable: true,
        // colour: "Green",
        colour: "No precipitate",
      },
      {
        name: "Iron (II) Carbonate",
        soluable: false,
        colour: "Grey",
      },
      {
        name: "Iron (II) Hydroxide",
        soluable: false,
        colour: "Green",
      },
      {
        name: "Iron (II) Chloride",
        soluable: true,
        // colour: "Green",
        colour: "No precipitate",
      },
      {
        name: "Iron (II) Bromide",
        soluable: true,
        // colour: "Green",
        colour: "No precipitate",
      },
      {
        name: "Iron (II) Iodide",
        soluable: true,
        // colour: "Green",
        colour: "No precipitate",
      },
      {
        name: "Iron (II) Acetate",
        soluable: true,
        // colour: "Green",
        colour: "No precipitate",
      },
      {
        name: "Iron (III) Phosphate",
        soluable: false,
        colour: "Yellow",
      },
      {
        name: "Iron (III) Sulfate",
        soluable: true,
        // colour: "Yellow",
        colour: "No precipitate",
      },
      {
        name: "Iron (III) Hydroxide",
        soluable: false,
        colour: "Brown",
      },
      {
        name: "Iron (III) Chloride",
        soluable: true,
        // colour: "Brown",
        colour: "No precipitate",
      },
      {
        name: "Iron (III) Bromide",
        soluable: true,
        // colour: "Brown",
        colour: "No precipitate",
      },
      {
        name: "Iron (III) Acetate",
        soluable: false,
        colour: "Brown",
        info: "Slightly soluable",
      },
      {
        name: "Silver Phosphate",
        soluable: false,
        colour: "Yellow",
      },
      {
        name: "Silver Sulfate",
        soluable: false,
        colour: "White",
        info: "Slightly soluable",
      },
      {
        name: "Silver Carbonate",
        soluable: false,
        colour: "Yellow",
      },
      {
        name: "Silver Chloride",
        soluable: false,
        colour: "White",
      },
      {
        name: "Silver Bromide",
        soluable: false,
        colour: "Yellow",
      },
      {
        name: "Silver Iodide",
        soluable: false,
        colour: "Yellow",
      },
      {
        name: "Silver Acetate",
        soluable: false,
        colour: "White",
        info: "Slightly soluable",
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
        flame: "No characteristic flame colour",
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
    this.nextQuestion();
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
      if (this.random(2) == 0) {
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
                      ]
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
                      ]
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
                      ]
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
                      ]
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
        let aspects = ["soluable", "colour"];
        // console.log(aspects);
        // console.log(aspects);
        let aspect = aspects[this.random(aspects.length)];
        console.log(aspect);
        // console.log(aspect);
        switch (aspect) {
          case "soluable":
            question = obj.name + " is soluable.";
            answer = String(obj.soluable);
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
                      ]
                    );
                  },
                });
              } else {
                actions.push({
                  title: choice,
                  type: "normal",
                  handler: () => {
                    this.$alert.present("Correct", "The answer is " + answer, [
                      {
                        title: "Next Question",
                        type: "normal",
                        handler: () => {
                          this.nextQuestion();
                        },
                      },
                    ]);
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
                      ]
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
                      ]
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
