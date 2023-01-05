### CodeWriter Packages ![Stars](https://img.shields.io/github/stars/codewriter-packages?style=social)

<hr>

## [Tri Inspector](https://github.com/codewriter-packages/Tri-Inspector) &middot; ![GitHub Repo stars](https://img.shields.io/github/stars/codewriter-packages/Tri-Inspector?style=flat-square) [![Github license](https://img.shields.io/github/license/codewriter-packages/Tri-Inspector.svg?style=flat-square)](#) ![GitHub package.json version](https://img.shields.io/github/package-json/v/codewriter-packages/Tri-Inspector?style=flat-square)
Free and open-source library that improves unity inspector.

<hr>

## [UniMob](https://github.com/codewriter-packages/UniMob) &middot; ![GitHub Repo stars](https://img.shields.io/github/stars/codewriter-packages/unimob?style=flat-square) [![Github license](https://img.shields.io/github/license/codewriter-packages/UniMob.svg?style=flat-square)](#) ![GitHub package.json version](https://img.shields.io/github/package-json/v/codewriter-packages/UniMob?style=flat-square)
Modern reactive programming library. UniMob inspired by [MobX](https://github.com/mobxjs/mobx) and adapts the principles of object-oriented reactive programming for Unity.

```csharp
// declare reactive property
[Atom] private int Counter { get; set; }

// Print message when Counter changed until Lifetime terminated
Atom.Reaction(Lifetime, () => Debug.Log("Tap count: " + Counter));
```

<hr>

## [UniMob.UI](https://github.com/codewriter-packages/unimob.ui) &middot; ![GitHub Repo stars](https://img.shields.io/github/stars/codewriter-packages/unimob.ui?style=flat-square) [![Github license](https://img.shields.io/github/license/codewriter-packages/UniMob.UI.svg?style=flat-square)](#) ![GitHub package.json version](https://img.shields.io/github/package-json/v/codewriter-packages/UniMob.UI?style=flat-square)
MVU/MVI/Redux like library for building declarative user interface in Unity. Built over [UniMob](https://github.com/codewriter-packages/UniMob). Inspired by [Flutter](https://github.com/flutter/flutter).

```csharp
private Widget BuildTodos(BuildContext context) {
    return new ScrollList {
        MainAxisAlignment = MainAxisAlignment.Start,
        CrossAxisAlignment = CrossAxisAlignment.Center,
        Children = {
            _todoList.Todos.Where(todo => todo.Finished).Select(todo => new TodoWidget(todo.Id))
        }
    };
}
```

> More examples can be found in the **[UniMob.UI Samples](https://github.com/codewriter-packages/UniMob.UI-Samples#readme)** repository

<hr>

### More packages
- `Animation` [Mesh-Animation](https://github.com/codewriter-packages/Mesh-Animation)  - *Fast GPU vertex shader based animation library for Unity;*
- `UI` [View-Binding](https://github.com/codewriter-packages/View-Binding) - *View binding library for Unity;*
- `UI` [Style-Components](https://github.com/codewriter-packages/Style-Components) - *Library for styling game objects in Unity;*
- `Utilities` [Expression-Parser](https://github.com/codewriter-packages/Expression-Parser) - *Simple math expression parser library for Unity;*
- `ECS` [Morpeh.Events](https://github.com/codewriter-packages/Morpeh.Events) - *Events for Morpeh ECS;*
- `ECS` [Morpeh.SystemStateProcessor](https://github.com/codewriter-packages/Morpeh.SystemStateProcessor) - *Reactivity for Morpeh ECS;*
- `ECS` `OBSOLETE` ~~[Morpeh.StateMachine](https://github.com/codewriter-packages/Morpeh.StateMachine) - *StateMachine for Morpeh ECS;*~~
- `ECS` `OBSOLETE` ~~[Morpeh-UniMob-Globals](https://github.com/codewriter-packages/Morpeh-UniMob-Globals)~~
- `Editor` [Package-Symlinker](https://github.com/codewriter-packages/Package-Symlinker) - *Utility that simplifies UPM package development;*
- `Editor` [NpmPublisherSupport](https://github.com/codewriter-packages/NpmPublisherSupport) - *Publish Npm packages to your registry directly from the Unity;*
- `Editor` `OBSOLETE` ~~[NpmPackageLoader](https://github.com/codewriter-packages/NpmPackageLoader) - *Pack assets to UnityPackages and distribute them via npm registry;*~~
- `Samples` [MVC-for-UI-Cookbook](https://github.com/codewriter-packages/MVC-for-UI-Cookbook) - *MVC templates for Unity with various frameworks;*
- `Samples` [UniMob.UI-Samples](https://github.com/codewriter-packages/UniMob.UI-Samples) - *Samples for UniMob.UI;*
- `Samples` `OBSOLETE` ~~[SampleApp-Clicker](https://github.com/codewriter-packages/SampleApp-Clicker) - *Sample app uses UniMob, UniMob.UI, View-Binding, Style-Components, Morpeh, Morpeh-UniMob-Globals;*~~
