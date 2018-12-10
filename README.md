# ui-language-spec
User Interaction Language Specification

# User Interaction Language Specification

Standards and the language specifications for writing acceptance criteria for web components.

## Concepts
### Acceptance criteria
> What it is.
> What it can do.
> What is this.
> Where will this be used.
> Why do we need a standard

All this is to build an User interaction design language. Ideal result of this whatever is to be able to develop web components from a text. This will be similar to GHERKIN syntax, but with reduced noise.

> If you understand it, if this proposal is not satisfactory for you, please share your idea to solve this better.

## Problem statement
I need a solution to build a component from a human understandable text. 
This language should be understood easily by users, developers, the great management fellows.(innocent, what-am-i, cunning).
More importantly it should be understood by a program which is definetely not a AI powered logic but a human developer writen logic. This way we can have wider range of developers to share and understand how this all work.

## Solution
A program that can read a standardazed acceptance criteria and generate a code as well.
## Terminologies
### Acceptance criteria
A set of steps containing EVENT/ACTION(of element/utility/component) EXPECT visibility/position. 

### Element
A valid html element that can show information and interactable.
This can dispatch Event.
This has State.

### Event
Carries message from an Element to Utilities and Components.

### State
Represents the visual information of a Component/Element.
An Element/Component with difrerent states will have different visuals.

### Component
Composed of two or more Elements or Components. This has a state.
This can dispatch Action and subscribe to Events and Actions.
This has State.

### Action
Carries message from Component and delivers to whoever subscribed to it. Triggers a state change for everyone attached to the action. 

#### Question
Which order the state changes should happen for the component - from the source then destination?
If a component is a subcomponent, state change in parent component should take care of state change in the child component.
If two components are sibblings, state change should happen to its parent component.
In any case, state change should be triggered in the parent level.

> Timing/ animation are all part of css that is another problem to solve not now.

### Not important
If you have suggestion to improve current proposal, please feel free to start creating one of your own rather than throwing your ideas here. Show off this standards be evolved into much better one by creating your own project. If it sounds better wise move would be to abandon this and contribute to yours. This can be applied to any framework on the basis of how you organise the code. This standard should also help in generating framework specific code.

#### Getting Started

#### Progress
- [x] Document the writings to a github readme.md
- [ ] ACs.
    - [ ] Write the standards.
    - [ ] Provide examples.
    - [ ] Provide a separate article/page for step by step
- [ ] UI Editor.
    - [ ] Share the wireframe.
    - [ ] AC
        - [ ] It should have a elements tab.
        - [ ] It should have a components tab.
        - [ ] Element
            - [ ] On click of new element - markup editor should show up.
            - [ ] Element should have Event section.
            - [ ] Element and should have State section.
        - [ ] Component
            - [ ] On click of new component - markup editor with should show up with only elements that are avaialble.
            - [ ] Component should have a Action section.
            - [ ] Component should have a state section.
        - [ ] Event section should contain list of events that this element is expected to dispatch.
        - [ ] State section should help to create new element state. 
- [ ] Put the photo that you have here.
- [ ] Build the UI Editor.
- [ ] Find out list of elements and few commonly used components.

#### Future
1. Write AC validator.
2. Write AC generator.

## Contributing

Project did on plan on helping the contributors yet. If you know what to do, and the impact it can make, you dont need help.

## Versioning

Project needs some versioning standards. Please provide it as a suggestion in the issue tab.

## Authors

* **Vetrivel Shanmugam** - *Initial work* - [imvetri](https://github.com/imvetri)

See also the list of [contributors](https://github.com/your/project/contributors) who participated in this project.

## License

This project is licensed under no license.

## Acknowledgments

* Hat tip to anyone whose code was used
* Inspiration
* etc
