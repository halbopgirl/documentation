---
sidebar_position: 2
---

# Popup Modal Component

Modal That Pops Open when a Button is Selected and can be Closed using the Close Button:

## PopupModal.js Code

```jsx title="PopupModal.js"
<div>
  <button className="popup-modal-button" onClick={e => {showModal()}}>Open Popup Modal</button>
  {shownModal ? 
    <div className={props.darkMode ? "popup-modal dark-mode" : "popup-modal"}>
      <button className="close-button" data-testid="close-button" onClick={e => {closeModal()}}>X</button>
      <div className="popup-modal-content">
          <h1>{props.header}</h1>
          <div>{props.content}</div>
      </div>
    </div> 
    : <div />
  }
</div>
```

## Props Included
- header: a string to pass in the name of the header within the modal
- content: a node, to pass in the React/HTML content of the modal
- darkMode: allows the user to choose whether the styling of the modal is in light mode or dark mode

## Variables Included
- shownModal: a boolean that tells the DOM whether to render the modal or an empty div