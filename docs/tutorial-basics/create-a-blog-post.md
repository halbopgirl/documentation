---
sidebar_position: 3
---

# Tooltip Modal Component

Modal That Pops Open when Text is Hovered

## ToolTipModal.js Code

```jsx title="ToolTipModal.js"
<div>
  <div className="tooltip-label" ref={ref}><p>Tooltip Modal</p></div>
  {showTooltipModal ? 
    <div className={props.darkMode ? "tooltip-modal dark-mode" : "tooltip-modal"}>
      <div className="little-square" />
      <div className="tooltip-modal-content">
        <h1 className="tooltip-header">{props.header}</h1>
        {props.content}
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