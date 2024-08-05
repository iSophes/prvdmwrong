<div align="center">
<img
  align="center"
  src="./assets/wordmark-dark.svg#gh-dark-mode-only"
  alt="Prvd 'M Wrong"
  width="500px"/>
<img
  align="center"
  src="./assets/wordmark-light.svg#gh-light-mode-only"
  alt="Prvd 'M Wrong"
  width="500px"/>

<br/>

![Continuous Integration](https://img.shields.io/github/actions/workflow/status/team-fireworks/prvdmwrong/ci.yml?style=flat-square&label=Continuous%20Integration)
![GitHub Actions Workflow Status](https://img.shields.io/github/actions/workflow/status/team-fireworks/prvdmwrong/docs.yml?style=flat-square&label=Documentation)
</br>
![GitHub License](https://img.shields.io/github/license/team-fireworks/prvdmwrong?style=flat-square)
![Made with Prvd 'M Wrong](https://img.shields.io/badge/made_with-prvd_'m_wrong-orange?style=flat-square&color=%23E26600)
</br>
<a href="https://team-fireworks.github.io/prvdmwrong/latest/reference">Website</a> ·
<a href="https://team-fireworks.github.io/prvdmwrong/latest/reference">Reference</a> ·
<a href="CHANGELOG.md">Changelog</a> ·
<a href="CONTRIBUTING.md">Contributing</a>
</div>

Prvd 'M Wrong is a game framework for a next-generation Roblox.

Sounds boring. Let's do that again.

***Prvd 'M Wrong will not make you a front page developer, but you may feel like
one.***

Once installed, your game will become your money back. Prvd 'M Wrong accelerates
the process with providers, connecting the top-level design of your game. Choose
to mix in networking and components as you need. Cherish a development
experience that fades into the background, freeing you to build faster and
**prvd 'm wrong.** It's the swaggest framework in town!

Sparked your interest? [Get going in minutes with our on-rails
tutorial.](https://team-fireworks.github.io/prvdmwrong/latest/tutorials/)

## Highlights

- Type-safe APIs for both Luau and TypeScript
- Featherlight, choose to mix in packages as you need
- Uses dependency injection for cleaner code organization
- Made to be extendable through modding APIs
- Non-intrusive first-class lifecycle events for flexibility
- Designed for clarity

## Code Sample

```Luau
local prvd = require("@pkg/prvdmwrong")
local CharacterProvider = require("./character-provider")

local CombatProvider = {}
type Self = typeof(CombatController)
CombatProvider.characterProvider = prvd.use(CharacterProvider)

function CombatProvider:onStart()
  print("Hello, Prvd 'M Wrong!")
end

function CombatProvider.performMove(self: Self, move: CombatMove)
  local character = self.characterProvider:awaitCharacter()
  -- do something with the character
end

return prvd(CombatProvider)
```

```TypeScript
import { Provider, use } from "@rbxts/prvdmwrong"
import { CharacterProvider } from "./character-provider"

@Provider()
export class CombatProvider {
  public characterProvider: use(CharacterProvider)

  public onStart() {
    print("Hello, Prvd 'M Wrong!")
  }

  public performMove(move: CombatMove) {
    const character = this.characterProvider.awaitCharacter()
    // do something with the character
  }
}
```

## License

Prvd 'M Wrong is released under the MIT license. Go do cool stuff with it!
