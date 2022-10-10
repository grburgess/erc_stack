# What am I?

A simple stack to add bitlbee, signald, and discourse the ERC in emacs.

## Install

```sh
mkdir -p config/bitlbee && mkdir -p config/signald/run
docker-compse up -d
```


Enter into the signald container and sign into the account

```sh
docker exec -i <container id> bash
signaldctl account link

```
 Then load ERC in emacs pointed at localhost:6667

### Discord

 ```sh
account add discord <email> <password>
account discord on
chat list discord
chat add discord !<number> #<name>
save


 ```

 ### Signal

 ```sh

 account add hehoe-signald +<phone number>
 account hehoe-signald set tag signal
 account signal on
 account signal set nick_format %full_name-sig
 /msg friend-sig
 ```
