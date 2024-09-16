# NixOS Installation Instructions

To install this package on NixOS is rather easy.


First, you'll need to make a custom derivation. You use find the banana-cursor-dreams.nix inside of this repo.


Then inside of your home manager, you can define your cursor as follows:

```
home.pointerCursor = {
  x11.enable = true;
  gtk.enable = true;
  package = pkgs.banana-cursor-dreams;
  size = 96;
  name = "Banana-Catppuccin-Mocha"; # Change to whatever theme you like
};
```

For an example of how I do this, you can view my dotfiles at [elliottminns/dotfiles](https://github.com/elliottminns/dotfiles)
