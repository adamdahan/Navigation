# Navigation

- Simplifies UIViewController instantiation using only the controller StoryboardID. 
- Check the existence of a UIViewController in the project with the controller StoryboardID
- Return list name (file name) of Storyboard in project
- Return list name (StoryboardID) of UIViewController in project

## Installation

Import Navigation.swift in your project (or use example project)

## Usage 

Return a initialised UIViewController just with Name (Name is a StoryboardId)

```Swift
if let controller = Navigation.getViewController("MyController") {
self.navigationController?.pushViewController(controller, animated: true)
}
```

Verify if controller exist in project 

```Swift
if Navigation.controllerExist("MyController") {
print("MyController exist")
}
```

Return all storyboard name (file name)

```Swift
Navigation.getAllStoryboardName()
```
Return all UIViewController name (StoryboardID) 

```Swift
Navigation.getAllViewControllerName()
```
Return all UIViewController name (StoryboardID) for specific Storyboard

```Swift
Navigation.getAllViewController(inStoryboard: "Main")
```

