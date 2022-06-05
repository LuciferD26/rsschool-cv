# Maksim Pryshchep
#### Junior Software Engineer JavaScript/Front-end
***
#### Contact information:

* **Phone:** +48733095261  
* **E-mail:** m.prishep@gmail.com  
* **Telegram:** @Maksim260488
* **Discord:** Maksim Pryshchep (LuciferD26)
* **Githab:** https://github.com/LuciferD26/
***
## About Me
Hi all. I'm 34 years old. I have been fond of computer technologies for a long time (just as an amateur), and now I decided to change my life and connect myself with IT.
***
## Skills

* HTML5, CSS3 (BEM)
* JavaScript Basics
* GitHub
* Figma, Adobe Photoshop, Adobe Photoshop Lightroom
***
## Code Examples
```
const openModalButton = document.querySelector('.profile__edit-button');
const closeModalButton = document.querySelector('.modal__close-button');
const modal = document.querySelector('.modal');
const form = document.querySelector('.form');
const inputName = document.querySelector('.form__input_type_name');
const inputProfession = document.querySelector('.form__input_type_profession');
const profileName = document.querySelector('.profile__name');
const profileProfession = document.querySelector('.profile__profession');

function toggleModal() {
  modal.classList.toggle('modal_open');
}

function profileContentEdit(event) {
  event.preventDefault();
  profileName.textContent = inputName.value;
  profileProfession.textContent = inputProfession.value;
  toggleModal();
}

function profileContent() {
  inputName.value = profileName.textContent;
  inputProfession.value = profileProfession.textContent;
  toggleModal();
}

closeModalButton.addEventListener('click', toggleModal);

form.addEventListener('submit', profileContentEdit);

openModalButton.addEventListener('click', profileContent);
```