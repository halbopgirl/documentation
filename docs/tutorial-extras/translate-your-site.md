---
sidebar_position: 2
---

# Testing

There is 100% code coverage when unit testing existing components with Jest.

## Test Example

ToolTip Modal Test:

```js title="TooltopModal.test.js"
test('renders tooltip modal', () => {
      const tooltip = render(<ToolTipModal
        header='Tooltip Modal Header'
        content={<div className="tooltip-modal"><p>text</p></div>}
        darkMode={false}
      />);
      
      const linkElement = screen.getByText("Tooltip Modal");
      expect(linkElement).toBeInTheDocument();
      userEvent.hover(linkElement);
      const modalElement = screen.getByText("Tooltip Modal Header");
      expect(modalElement).toBeVisible();
      userEvent.unhover(linkElement);
      expect(modalElement).not.toBeVisible();
});
```

## Types of testing

Multiple Types of Tests are Run, Including:
- Checking document for text
- Expecting text to be visible
- Testing hover action functionality
- Testing click action functionality
- Checking for a particular class name

