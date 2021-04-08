FROM nixos/nix

ADD nix.conf /etc/nix/nix.conf

RUN nix-channel --add https://nixos.org/channels/nixpkgs-unstable nixpkgs
RUN nix-channel --update

# RUN nix-build -A git '<nixpkgs>'
RUN nix-env -i git cabal-install stack ghc docker
