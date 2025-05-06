<template>
    <div class="modaldiv">
      <h2>Baluster Quantity Calculator</h2>
      <div class="row align-items-start d-flex align-items-center mt-5 mb-5">
        <p>
          As part of my work with DecksGo, I developed a <strong>custom JavaScript application</strong> that helps customers calculate the number of balusters they need based on their deck section lengths and desired spacing. Starting with only a <strong>basic formula</strong>, I transformed it into an interactive tool with dynamic input fields, real-time validation, and result calculation.
        </p>

        <p>
          To enhance usability, I <strong>designed intuitive diagrams</strong> that visually explain how section length and spacing affect baluster quantity. The tool not only improves customer experience but also reduces product ordering errors.
        </p>

        <p>
          I <strong>styled the calculator for clarity and responsiveness</strong>, ensuring it works well across devices, and I <strong>embedded it directly into our Shopify store</strong> using CodePen and Nuxt.js, making it easily accessible to DIYers and contractors shopping online.
        </p>
        <p><strong>Try it yourself:</strong></p>

        <iframe src="https://decksgo-baluster-calculator.netlify.app/" class="detailsframe" style="height:800px;"></iframe>

        <div class="col-12 col-md-6">
          <p>
            The calculator uses a straightforward formula to estimate the number of balusters needed per deck section. Each section's total length (in inches) is divided by the combined width of a baluster and the desired spacing between balusters. In the code, this is represented as:
            <code>Math.ceil(sectionLength / (balusterWidth + spacing) - 1)</code>,
            where the <code>balusterWidth</code> is fixed at <strong>0.75 inches</strong> (standard width), and the spacing is user-defined (up to a max of 4"). The result is rounded up to ensure full coverage. This math is run dynamically for each section the user inputs, and the calculator totals all sections to output a final baluster count.
          </p>
          <p>
            You can see this logic in action directly in the embedded CodePen beside this explanation. It responds instantly to user input, updating the result as new section lengths or spacing values are entered.
          </p>
        </div>
        <div class="col-12 col-md-6 mt-5 mb-5">
            <p class="codepen detailsframe" data-height="500" data-default-tab="html,result" data-slug-hash="oggdOoN" data-pen-title="Untitled" data-user="Gree0638" style="height: 300px; box-sizing: border-box; display: flex; align-items: center; justify-content: center; border: 2px solid; margin: 1em 0; padding: 1em;">
              <span>See the Pen <a href="https://codepen.io/Gree0638/pen/oggdOoN">
              Untitled</a> by Tanner Green (<a href="https://codepen.io/Gree0638">@Gree0638</a>)
              on <a href="https://codepen.io">CodePen</a>.</span>
            </p>
        </div>
      </div>
    </div>
  </template>

<script setup>
  import { onMounted } from 'vue'

  onMounted(() => {
    const script = document.createElement('script')
    script.src = 'https://public.codepenassets.com/embed/index.js'
    script.async = true
    document.body.appendChild(script)
  })
</script>

<style scoped lang="css">
    .modaldiv {
        margin-left: 10%;
        margin-right: 10%;
        color: white;
        font-size: 1.2rem;
        line-height: 1.6;
    }

    img {
        width: 100%;
        border-radius: 20px;
    }

  iframe {
    border-radius: 20px;
  }


    @media screen and (max-width: 768px) {
      .modaldiv {
        margin-left: 10px;
        margin-right: 10px;
    }

        iframe {
          width: 100%;
        }

        p {
          padding-top: 20px;
          padding-bottom: 20px;
        }
    }
</style>