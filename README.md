# pythoneda-shared-git/github

Definition for [pythoneda-shared-git](https://github.com/pythoneda-shared-git "pythoneda-shared-git")/[git](https://github.com/pythoneda-shared-git/github "github").

## How to declare it in your flake

Check the latest tag of this repository, and use it instead of the `[version]` placeholder below.

```nix
{
  description = "[..]";
  inputs = rec {
    [..]
    pythoneda-shared-git-github = {
      [optional follows]
      url =
        "github:pythoneda-shared-git-def/github/[version]";
    };
  };
  outputs = [..]
};
```

Should you use another PythonEDA modules, you might want to pin those also used by this project. The same applies to [nixpkgs](https://github.com/nixos/nixpkgs "nixpkgs") and [flake-utils](https://github.com/numtide/flake-utils "flake-utils").

Use the specific package depending on your system (one of `flake-utils.lib.defaultSystems`) and Python version:

- `#packages.[system].pythoneda-shared-git-github-python38` 
- `#packages.[system].pythoneda-shared-git-github-python39` 
- `#packages.[system].pythoneda-shared-git-github-python310` 
- `#packages.[system].pythoneda-shared-git-github-python311`
