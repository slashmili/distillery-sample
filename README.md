# Myapp

```
$ mix release --verbose --profile=myapp:prod
==> mydist
Compiling 1 file (.ex)
Generated mydist app
==> myapp
Compiling 1 file (.ex)
Generated myapp app
==> Loading configuration..
==> Assembling release..
==> Building release myapp:0.1.0 using environment prod
==> Discovered applications:
  sasl-3.0
    from: /usr/local/Cellar/erlang/19.0.2_1/lib/erlang/lib/sasl-3.0
    applications:
      :kernel
      :stdlib
    includes: none

  iex-1.3.2
    from: /usr/local/Cellar/elixir/1.3.2/bin/../lib/iex
    applications:
      :kernel
      :stdlib
      :elixir
    includes: none

  myapp-0.1.0
    from: _build/dev/lib/myapp
    applications:
      {:uuid, :load}
      {:mydist, :load}
      :kernel
      :stdlib
      :elixir
      :logger
    includes:
      :uuid
  uuid-1.1.5
    from: _build/dev/lib/uuid
    applications:
      :kernel
      :stdlib
      :elixir
    includes: none

  kernel-5.0
    from: /usr/local/Cellar/erlang/19.0.2_1/lib/erlang/lib/kernel-5.0
    applications: none
    includes: none

  stdlib-3.0.1
    from: /usr/local/Cellar/erlang/19.0.2_1/lib/erlang/lib/stdlib-3.0.1
    applications:
      :kernel
    includes: none

  elixir-1.3.2
    from: /usr/local/Cellar/elixir/1.3.2/bin/../lib/elixir
    applications:
      :kernel
      :stdlib
      :compiler
    includes: none

  compiler-7.0.1
    from: /usr/local/Cellar/erlang/19.0.2_1/lib/erlang/lib/compiler-7.0.1
    applications:
      :kernel
      :stdlib
    includes: none

  mydist-0.1.0
    from: _build/dev/lib/mydist
    applications:
      {:uuid, :load}
      :kernel
      :stdlib
      :elixir
      :logger
    includes:
      :uuid
  logger-1.3.2
    from: /usr/local/Cellar/elixir/1.3.2/bin/../lib/logger
    applications:
      :kernel
      :stdlib
      :elixir
    includes: none

==> Generated overlay vars:
    release_name=:myapp
    release_version="0.1.0"
    is_upgrade=false
    upgrade_from=:latest
    dev_mode=false
    include_erts=true
    include_src=false
    include_system_libs=true
    erl_opts=""
    erts_vsn="8.0.2"
    output_dir="rel/myapp"
==> Copying applications to rel/myapp
==> Generating nodetool
==> Generating start_erl.data
==> Generating vm.args
==> Generating sys.config from config/config.exs
==> Including ERTS 8.0.2 from /usr/local/Cellar/erlang/19.0.2_1/lib/erlang/erts-8.0.2
==> Generating boot script
==> Failed to build release:

    Duplicated application included:
    	uuid included in myapp and mydist```
