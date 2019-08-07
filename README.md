# SLDS
## Form Elements
### Structure
To create a form element, a <div> element with the class slds-form-element is required.
A form element is made up of three primary elements, the label (slds-form-element__label), a container (slds-form-element__control), and the form element, i.e. <input>.



## Dreamforce Demo
This repository contains the demo code from our Dreamforce '18 talk for [Building Custom Lightning Components with the Lightning Design System](https://www.youtube.com/watch?v=-Ytt0HcbmxU)

## Files

### copyPastedExpressionBlueprint.cmp

This file contains the code we copied from the Lightning Design System's [Expression Blueprint page](https://lightningdesignsystem.com/components/expression/)
- The only changes we made were switching out the SVGs with [lightning:icon](https://developer.salesforce.com/docs/component-library/bundle/lightning:icon/example) and removing the "Add Group" button since we didn't need it for the demo
- This code is the starting point in the demo

### expressionBlueprintUsingLightningComponents.cmp

This file shows how to replace the pieces of the blueprint with existing lightning components, as diagrammed in this [slide from the demo](https://youtu.be/-Ytt0HcbmxU?t=671)

![Diagram showing Expression Blueprint broken down into Comboboxes, Inputs, Buttons, and Button Icons](/assets/ExpressionBrokenDown.png)

## Next Steps

`expressionBlueprintUsingLightningComponents.cmp` is a good starting point for building a fully functional Expression Component that responds to user input and utilizes the resulting data

Some next steps might include:
1. Customize the aura attributes and input labels to be specific to your use case
2. Create a new `ExpressionRow` component that you could use to dynamically create rows when the "Add Condition" button is clicked
3. Add JavaScript to implement the "Delete Condition" and "Add Condition" buttons
4. Implement the Submit button, which might iterate through your `ExpressionRow` components to grab the user selected values and store that data

## Resources

Helpful Trailhead modules:
1. [Lightning Design System](https://trailhead.salesforce.com/en/modules/lightning_design_system)
2. [UX Prototyping Basics](https://trailhead.salesforce.com/en/modules/ux-prototyping-basics)
3. [Build a Lightning App with the Lightning Design System](https://trailhead.salesforce.com/en/projects/slds-lightning-components-workshop)
4. [Build a Lightning Component to Override a Standard Action](https://trailhead.salesforce.com/en/projects/workshop-override-standard-action)
5. [Lightning App Builder](https://trailhead.salesforce.com/en/modules/lightning_app_builder)
