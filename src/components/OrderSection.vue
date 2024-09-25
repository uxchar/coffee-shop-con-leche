<script setup></script>
<template>
  <div class="order-section">
    <h2 class="order-title">What can we brew for you today?</h2>
    <div class="cust-info-section">
      <form action="#">
        <div class="name-section">
          <label for="fname" class="name-label">Your Name</label>
          <div class="customer-input-section">
            <input
              type="text"
              id="fname"
              name="fname"
              placeholder="First name"
            />
            <input
              type="text"
              id="lname"
              name="lname"
              placeholder="Last name"
            />
          </div>
        </div>
        <div class="email-section">
          <label for="email">Email address</label>
          <input
            type="text"
            id="email"
            name="email"
            placeholder="Eg example@email.com"
          />
        </div>
        <div class="phone-section">
          <label for="phone">Phone number</label>
          <input
            type="text"
            id="phone"
            name="phone"
            placeholder="Eg (555) 555-5555"
          />
        </div>
        <div class="cust-choice-section">
          <div class="drink-choice">
            <label for="liquad" class="drink-choice-title">Drink Choice</label>
            <label for="coffee">
              <input type="radio" id="coffee" name="liquad" value="coffee" />
              Coffee
            </label>
            <label for="black-tea">
              <input
                type="radio"
                id="black-tea"
                name="liquad"
                value="black-tea"
              />
              Black Tea
            </label>
            <label for="green-tea">
              <input
                type="radio"
                id="green-tea"
                name="liquad"
                value="green-tea"
              />
              Green Tea
            </label>
            <label for="americano">
              <input
                type="radio"
                id="americano"
                name="liquad"
                value="americano"
              />
              Americano
            </label>
            <label for="latte">
              <input type="radio" id="latte" name="liquad" value="latte" />
              Latte
            </label>
            <label for="mocha">
              <input type="radio" id="mocha" name="liquad" value="mocha" />
              Mocha
            </label>
          </div>
          <div class="shot-choice">
            <label for="shot" class="drink-choice-title second-title"
              >Shot Choice</label
            >
            <label for="espresso">
              <input
                type="checkbox"
                id="espresso"
                name="shot"
                value="espresso"
              />
              Espresso
            </label>
            <label for="caramel">
              <input type="checkbox" id="caramel" name="shot" value="caramel" />
              Caramel
            </label>
            <label for="hazelnut">
              <input
                type="checkbox"
                id="hazelnut"
                name="shot"
                value="hazelnut"
              />
              Hazelnut
            </label>
            <label for="no-shot">
              <input type="checkbox" id="no-shot" name="shot" value="no-shot" />
              No Shot
            </label>
          </div>
          <div class="milk-choice">
            <label for="milk" class="drink-choice-title third-title"
              >Milk Choice</label
            >
            <label for="whole-milk">
              <input
                type="checkbox"
                id="whole-milk"
                name="milk"
                value="whole-milk"
              />
              Whole Milk
            </label>
            <label for="oat-milk">
              <input
                type="checkbox"
                id="oat-milk"
                name="milk"
                value="oat-milk"
              />
              Oat Milk
            </label>
            <label for="soy-milk">
              <input
                type="checkbox"
                id="soy-milk"
                name="milk"
                value="soy-milk"
              />
              Soy Milk
            </label>
            <label for="no-milk">
              <input type="checkbox" id="no-milk" name="milk" value="no-milk" />
              No Milk
            </label>
          </div>
        </div>
        <div class="notes-section">
          <h2 class="note-title">Notes</h2>
          <textarea
            name="drink-notes"
            id="cust-notes"
            rows="10"
            cols="100"
            placeholder="Any allergies, additions, or other information for your order?"
          ></textarea>
        </div>
        <button type="submit" value="submit" class="submit-btn">
          Place Order
        </button>
      </form>
    </div>
  </div>
</template>

<style scoped>
form {
  margin-bottom: 100px;
  display: flex;
  flex-direction: column;
}

label {
  text-transform: uppercase;
  font-size: 0.9rem;
  margin-bottom: 15px;
}

input[type="text"] {
  max-width: 100%;
  height: 50px;
  margin: auto 20px 30px 0px;
  padding-left: 10px;
  border: 1px solid #ffffff;
  border-radius: 2px;
  background-color: #ffffff;
}

input[type="radio"],
input[type="checkbox"] {
  appearance: none;
  background-color: #fff;
  margin-right: 5px;
  width: 1.15em;
  height: 1.15em;
  border: 0.15em solid #fff;
  border-radius: 50%;
  transform: translateY(-0.075em);
  vertical-align: middle;
}

input[type="radio"]:checked {
  transform: scale(1);
  background-color: #0e2a54;
}
input[type="radio"]:focus {
  outline: max(2px, 0.15em) solid rgb(246, 211, 108);
  outline-offset: max(2px, 0.15em);
}

input[type="checkbox"] {
  border-radius: 0.15em;
}

input[type="checkbox"]:checked {
  transform: scale(1);
  color: #0e2a54;
  background-color: #fff;
  clip-path: polygon(14% 44%, 0 65%, 50% 100%, 100% 16%, 80% 0%, 43% 62%);
}

.order-section {
  display: flex;
  flex-direction: column;
  background-color: #0e2a54;
  color: rgb(255, 229, 151);
  padding-left: 30px;
  padding-right: 30px;
}
.order-title {
  font-size: 1.7rem;
  margin: 60px auto 40px auto;
}

.cust-info-section {
  display: flex;
  flex-direction: column;
  justify-content: center;
}
#fname,
#lname {
  width: 400px;
}
.name-section,
.email-section,
.phone-section {
  display: flex;
  flex-direction: column;
}

.name-label {
}

.cust-choice-section {
  display: flex;
  flex-direction: column;
  margin-bottom: 60px;
}

.drink-choice-title {
  margin: 15px auto;
}

.drink-choice,
.shot-choice,
.milk-choice {
  display: flex;
  flex-direction: column;
}

#cust-notes {
  border: 1px solid #e7e7e7;
  border-radius: 2px;
  margin-top: 10px;
  padding-left: 10px;
  padding-top: 10px;
  width: 100%;
}

.submit-btn {
  width: 100%;
  max-width: 500px;
  font-size: 1.1rem;
  border-radius: 6px;
  border-style: none;
  padding: 20px 15px;
  background-color: rgb(246, 211, 108);
  font-family: "Piazzolla", serif;
  font-weight: 700;
  white-space: nowrap;
  text-transform: capitalize;
  margin: 40px auto;
  justify-content: center;
  align-items: center;
}

@media screen and (min-width: 768px) {
  .order-section {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    background-color: #0e2a54;
    color: rgb(255, 229, 151);
  }

  .order-title {
    font-size: 3.3rem;
    margin-bottom: 60px;
    margin-top: 40px;
    padding: 20px;
    width: fit-content;
    border-radius: 2px;
  }

  .name-input-section {
    flex-direction: row;
  }

  .cust-choice-section {
    display: flex;
    flex-direction: row;

    align-items: flex-start;
    gap: 100px;
    margin-bottom: 60px;
  }

  input[type="text"] {
    width: 400px;
  }
}
@media screen and (min-width: 1100px) {
  .cust-choice-section {
    flex-direction: row;
    align-items: flex-start;
    gap: 200px;
    margin-bottom: 60px;
  }
}
</style>
