# Rebar3 OTP Behavior Templates

## Setup

Do this only once:

```
mkdir -p ~/.config/rebar3/templates
git clone git@github.com:marianoguerra/rebar3_otp_templates.git ~/.config/rebar3/templates/rebar3_otp_templates
```

If there are updates in the repo with new templates you can update them locally with:

```
cd ~/.config/rebar3/templates/rebar3_otp_templates
git pull origin master
```

## Usage

Modules are created in the current directory.

### gen\_server

```
$ rebar3 new gen_server name=foo

===> Writing foo.erl
```

### gen\_statem

```
$ rebar3 new gen_statem name=foo

===> Writing foo.erl
```

### supervisor

```
$ rebar3 new supervisor name=sup child_name=sup_child

===> Writing sup.erl
```

## Notes

gen\_server template based on https://gist.github.com/sergium/e65a41d7e6956c436177
