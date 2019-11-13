# Rebar3 OTP Behavior Templates

[Rebar3](http://www.rebar3.org/) [Erlang](https://www.erlang.org/) [Templates](http://www.rebar3.org/docs/using-templates) for common [OTP](https://erlang.org/doc/design_principles/des_princ.html) [behaviors](http://erlang.org/doc/design_principles/des_princ.html#behaviours).

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

* gen\_server template based on https://gist.github.com/sergium/e65a41d7e6956c436177
* gen\_statem template based on https://gist.github.com/eproxus/28fd864e2ba607d13ed4f5abc89ca27a
* supervisor based on https://gist.github.com/eproxus/28fd864e2ba607d13ed4f5abc89ca27a and snippet from tsloughter
