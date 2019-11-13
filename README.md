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

```
$ rebar3 new gen_server name=foo

===> Writing foo.erl
```

Modules are created in the current directory.

## Notes

gen\_server template based on https://gist.github.com/sergium/e65a41d7e6956c436177
