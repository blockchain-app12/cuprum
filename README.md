# Cuprum

## Introduction

Cuprum is a distributed consensus platform with meta-consensus
capability. Cuprum not only comes to consensus about the state of its ledger,
like Bitcoin or Ethereum. It also comes to consensus about how the
protocol and the nodes should adapt and upgrade. 

sudo apt install -y rsync git m4 build-essential patch unzip wget pkg-config libgmp-dev libev-dev libhidapi-dev libffi-dev opam jq zlib1g-dev
# [install rust]
wget https://sh.rustup.rs/rustup-init.sh

chmod +x rustup-init.sh

./rustup-init.sh --profile minimal --default-toolchain 1.52.1 -y

# [source cargo]

source $HOME/.cargo/env

# [get sources]


opam init --bare

make build-deps

eval $(opam env)

make

