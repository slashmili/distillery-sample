# Myum

```
$ mix release --verbose --profile=myapp:prod
==> Loading configuration..
==> Assembling release..
==> Building release myapp:0.1.0 using environment prod
==> Discovered applications:
  mydist-0.1.0
    from: _build/dev/lib/mydist
    applications:
      kernel
      stdlib
      elixir
      logger
    includes: none

  sasl-3.0
    from: /usr/local/Cellar/erlang/19.0.2/lib/erlang/lib/sasl-3.0
    applications:
      kernel
      stdlib
    includes: none

  iex-1.3.2
    from: /usr/local/Cellar/elixir/1.3.2/bin/../lib/iex
    applications:
      kernel
      stdlib
      elixir
    includes: none

  myapp-0.1.0
    from: _build/dev/lib/myapp
    applications:
      kernel
      stdlib
      elixir
      logger
    includes: none

  kernel-5.0
    from: /usr/local/Cellar/erlang/19.0.2/lib/erlang/lib/kernel-5.0
    applications: none
    includes: none

  stdlib-3.0.1
    from: /usr/local/Cellar/erlang/19.0.2/lib/erlang/lib/stdlib-3.0.1
    applications:
      kernel
    includes: none

  elixir-1.3.2
    from: /usr/local/Cellar/elixir/1.3.2/bin/../lib/elixir
    applications:
      kernel
      stdlib
      compiler
    includes: none

  compiler-7.0.1
    from: /usr/local/Cellar/erlang/19.0.2/lib/erlang/lib/compiler-7.0.1
    applications:
      kernel
      stdlib
    includes: none

  logger-1.3.2
    from: /usr/local/Cellar/elixir/1.3.2/bin/../lib/logger
    applications:
      kernel
      stdlib
      elixir
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
==> Including ERTS 8.0.2 from /usr/local/Cellar/erlang/19.0.2/lib/erlang/erts-8.0.2
==> Generating boot script
==> Generating RELEASES
==> Generating start_clean.boot
==> Applying overlays
==> Applying mkdir overlay
    dst: releases/0.1.0/hooks
==> Applying mkdir overlay
    dst: releases/0.1.0/commands
==> Packaging release..
==> Archiving myapp-0.1.0
==> Writing tarball to rel/myapp/releases/0.1.0/myapp.tar.gz
==> Updating tarball
==> Tarball updated!
==> Release successfully built!
    You can run it in one of the following ways:
      Interactive: rel/myapp/bin/myapp console
      Foreground: rel/myapp/bin/myapp foreground
      Daemon: rel/myapp/bin/myapp start
$ rel/myapp/bin/myapp console
iex(myapp@127.0.0.1)1> Application.started_applications
[{:myapp, 'myapp', '0.1.0'}, {:iex, 'iex', '1.3.2'},
 {:sasl, 'SASL  CXC 138 11', '3.0'}, {:mydist, 'mydist', '0.1.0'},
 {:logger, 'logger', '1.3.2'}, {:elixir, 'elixir', '1.3.2'},
 {:compiler, 'ERTS  CXC 138 10', '7.0.1'},
 {:stdlib, 'ERTS  CXC 138 10', '3.0.1'}, {:kernel, 'ERTS  CXC 138 10', '5.0'}]
```
