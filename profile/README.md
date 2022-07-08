### CodeWriter Packages ![Stars](https://img.shields.io/github/stars/codewriter-packages?style=social)

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

> More examples can be found in the **[UniMob Samples](https://github.com/codewriter-packages/UniMob.UI-Samples#readme)** repository

<hr>

## [Tri Inspector](https://github.com/codewriter-packages/Tri-Inspector) &middot; ![GitHub Repo stars](https://img.shields.io/github/stars/codewriter-packages/Tri-Inspector?style=flat-square) [![Github license](https://img.shields.io/github/license/codewriter-packages/Tri-Inspector.svg?style=flat-square)](#) ![GitHub package.json version](https://img.shields.io/github/package-json/v/codewriter-packages/Tri-Inspector?style=flat-square)
Free and open-source library that improves unity inspector.
