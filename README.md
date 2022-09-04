<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta http-equiv="X-UA-Compatible" content="IE=edge" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>🥐</title>
  </head>
  <style>
    body {
      background: linear-gradient(115deg, rgb(0, 0, 0) 5.8%, rgb(178, 14, 14) 112.6%);
    }

    h2 {
      text-align: center;
      color: #5e1c03;
    }

    h1 {
      text-align: center;
      color: #ffe486;
      border: 1px solid #ffe486;
      border-radius: 4px;
      padding: 5px;
      line-height: 2;
      font-family: Cambria, Cochin, Georgia, Times, "Times New Roman", serif;
      font-weight: bold;
      font-size: 40px;
    }

    img {
      display: block;
      margin: 0 auto;
      border-radius: 50%;
      max-width: 100%;
      padding 10px;
    }

    p {
      line-height: 1.5;
      margin: 0;
      font-family:Cambria, Cochin, Georgia, Times, "Times New Roman", serif;
      font-size: 18px;
      color:#777755;
      font-style: italic;
      font-weight: bold;
      text-align: justify;
    }

    button {
      display: block;
      margin: 0 auto;
      padding: 20px;
      background-color:#5e1c03;
      color: #4C0606;
      font-size: 20px;
      font-weight: normal;
      font-family:Cambria, Cochin, Georgia, Times, "Times New Roman", serif;
      padding: 20px 30px;
      border: none;
      border-radius: 4px;
      box-shadow: 5px 5px 8px rgba(0, 0, 0, 0.5);
      transition: all 300ms ease-in-out;
    }
    button:hover {
      cursor: grab;
      background-color: #FFE486;
    }

    .read-more {
      display: block;
      font-weight: normal;
      font-size: 11px;
      font-family:Cambria, Cochin, Georgia, Times, "Times New Roman", serif;
      margin-top: 10px;
      text-decoration:none;
      color:#777755;
    }
    .read-more:hover {
      text-decoration: underline;
      cursor: pointer;
      transition: all 50ms ease-in-out;
      opacity: 0.5;
    }
    .wikipedia {
      font-weight: bold;
    }
    a {
      text-align: end;
    }

    hr {
      background-color: #430606;
      height: 1px;
      border: #4C0606;
    }
    .credits {
      text-align: center;
      font-family:Cambria, Cochin, Georgia, Times, "Times New Roman", serif;
      font-style: normal;
      font-size: 16px;
      color:#FFE486;
      padding: 30px;
      font-weight: normal;
    }
    .name {
      color: #FFE486;
    }
    .name:hover {
      cursor:help;
      opacity: 0.5;
    }

    .content {
      max-width: 600px;
      margin: 0 auto;
      padding: 5px 20px;
    }
  </style>
  <body>
    <div class="content">
      <h2><em>Sweet or salty</em></h2>
      <h1>Croissant</h1>
      <img
        src="https://s3.amazonaws.com/shecodesio-production/uploads/files/000/045/439/original/croissant-ma%C5%9Blany-70g.jpg?1662299672"
        alt="Croissant"
        width="400px"
      />
      <br />
      <p>
        A croissant is a buttery, flaky, French viennoiserie pastry inspired by
        the shape of the Austrian kipferl but using the French yeast-leavened
        laminated dough. Croissants are named for their historical crescent
        shape, the dough is layered with butter, rolled and folded several times
        in succession, then rolled into a thin sheet, in a technique called
        laminating. The process results in a layered, flaky texture, similar to
        a puff pastry.
        <a
          href="https://en.wikipedia.org/wiki/Croissant"
          target="_blank"
          class="read-more"
        >
          <em
            >Read more on
            <span class="wikipedia">Wikipedia</span>
          </em>
        </a>
        <br />
      </p>
      <button class="getButton">Get a croissant</button>
      <br />
      <hr />
      <p class="credits">
        🥐 Page written by
        <a href="https://github.com/beckyzaranko" target="_blank" class="name">
          Katia</a
        >
        🥐
      </p>
    </div>
    <script>
      function get() {
        let name = prompt("What is your name?");
        let like = prompt("Bonjour " + name + ". Do you like croissants?");
        like = like.toLowerCase();

        if (like === "no") {
          alert("Au revoir " + name + " 🥐");
        } else {
          let email = prompt("What is your email?");
          let flavor = prompt("What is your favourite flavor of croissant?");
          alert(
            "Bonjour " +
              name +
              ", " +
              flavor +
              " croissant will come to you. Thanks for contact!"
          );
        }
      }

      let getButton = document.querySelector(".getButton");
      getButton.addEventListener("click", get);
    </script>
  </body>
</html>

