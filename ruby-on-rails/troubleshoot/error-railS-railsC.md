# Troubleshoot: Error when run `rails server` or `rails console`

## Materials
* Rails v5.2.2

## Error
- $1 = computer user
- $2 = project path

```
Traceback (most recent call last):
	26: from bin/rails:4:in `<main>'
	25: from /Users/$1/.rbenv/versions/2.5.1/lib/ruby/gems/2.5.0/gems/activesupport-5.2.2.1/lib/active_support/dependencies.rb:291:in `require'
	24: from /Users/$1/.rbenv/versions/2.5.1/lib/ruby/gems/2.5.0/gems/activesupport-5.2.2.1/lib/active_support/dependencies.rb:257:in `load_dependency'
	23: from /Users/$1/.rbenv/versions/2.5.1/lib/ruby/gems/2.5.0/gems/activesupport-5.2.2.1/lib/active_support/dependencies.rb:291:in `block in require'
	22: from /Users/$1/.rbenv/versions/2.5.1/lib/ruby/gems/2.5.0/gems/bootsnap-1.4.1/lib/bootsnap/load_path_cache/core_ext/kernel_require.rb:29:in `require'
	21: from /Users/$1/.rbenv/versions/2.5.1/lib/ruby/gems/2.5.0/gems/bootsnap-1.4.1/lib/bootsnap/load_path_cache/core_ext/kernel_require.rb:20:in `require_with_bootsnap_lfi'
	20: from /Users/$1/.rbenv/versions/2.5.1/lib/ruby/gems/2.5.0/gems/bootsnap-1.4.1/lib/bootsnap/load_path_cache/loaded_features_index.rb:83:in `register'
	19: from /Users/$1/.rbenv/versions/2.5.1/lib/ruby/gems/2.5.0/gems/bootsnap-1.4.1/lib/bootsnap/load_path_cache/core_ext/kernel_require.rb:21:in `block in require_with_bootsnap_lfi'
	18: from /Users/$1/.rbenv/versions/2.5.1/lib/ruby/gems/2.5.0/gems/bootsnap-1.4.1/lib/bootsnap/load_path_cache/core_ext/kernel_require.rb:21:in `require'
	17: from /Users/$1/.rbenv/versions/2.5.1/lib/ruby/gems/2.5.0/gems/railties-5.2.2.1/lib/rails/commands.rb:18:in `<main>'
	16: from /Users/$1/.rbenv/versions/2.5.1/lib/ruby/gems/2.5.0/gems/railties-5.2.2.1/lib/rails/command.rb:46:in `invoke'
	15: from /Users/$1/.rbenv/versions/2.5.1/lib/ruby/gems/2.5.0/gems/railties-5.2.2.1/lib/rails/command/base.rb:65:in `perform'
	14: from /Users/$1/.rbenv/versions/2.5.1/lib/ruby/gems/2.5.0/gems/thor-0.20.3/lib/thor.rb:387:in `dispatch'
	13: from /Users/$1/.rbenv/versions/2.5.1/lib/ruby/gems/2.5.0/gems/thor-0.20.3/lib/thor/invocation.rb:126:in `invoke_command'
	12: from /Users/$1/.rbenv/versions/2.5.1/lib/ruby/gems/2.5.0/gems/thor-0.20.3/lib/thor/command.rb:27:in `run'
	11: from /Users/$1/.rbenv/versions/2.5.1/lib/ruby/gems/2.5.0/gems/railties-5.2.2.1/lib/rails/commands/server/server_command.rb:142:in `perform'
	10: from /Users/$1/.rbenv/versions/2.5.1/lib/ruby/gems/2.5.0/gems/railties-5.2.2.1/lib/rails/commands/server/server_command.rb:142:in `tap'
	 9: from /Users/$1/.rbenv/versions/2.5.1/lib/ruby/gems/2.5.0/gems/railties-5.2.2.1/lib/rails/commands/server/server_command.rb:145:in `block in perform'
	 8: from /Users/$1/.rbenv/versions/2.5.1/lib/ruby/gems/2.5.0/gems/activesupport-5.2.2.1/lib/active_support/dependencies.rb:291:in `require'
	 7: from /Users/$1/.rbenv/versions/2.5.1/lib/ruby/gems/2.5.0/gems/activesupport-5.2.2.1/lib/active_support/dependencies.rb:257:in `load_dependency'
	 6: from /Users/$1/.rbenv/versions/2.5.1/lib/ruby/gems/2.5.0/gems/activesupport-5.2.2.1/lib/active_support/dependencies.rb:291:in `block in require'
	 5: from /Users/$1/.rbenv/versions/2.5.1/lib/ruby/gems/2.5.0/gems/bootsnap-1.4.1/lib/bootsnap/load_path_cache/core_ext/kernel_require.rb:29:in `require'
	 4: from /Users/$1/.rbenv/versions/2.5.1/lib/ruby/gems/2.5.0/gems/bootsnap-1.4.1/lib/bootsnap/load_path_cache/core_ext/kernel_require.rb:20:in `require_with_bootsnap_lfi'
	 3: from /Users/$1/.rbenv/versions/2.5.1/lib/ruby/gems/2.5.0/gems/bootsnap-1.4.1/lib/bootsnap/load_path_cache/loaded_features_index.rb:83:in `register'
	 2: from /Users/$1/.rbenv/versions/2.5.1/lib/ruby/gems/2.5.0/gems/bootsnap-1.4.1/lib/bootsnap/load_path_cache/core_ext/kernel_require.rb:21:in `block in require_with_bootsnap_lfi'
	 1: from /Users/$1/.rbenv/versions/2.5.1/lib/ruby/gems/2.5.0/gems/bootsnap-1.4.1/lib/bootsnap/load_path_cache/core_ext/kernel_require.rb:21:in `require'
/Users/$1/$2/config/application.rb:18:in `<main>': undefined local variable or method `config' for main:Object (NameError)
```

## Instructions
In terminal:

- $3 = model name (singular)

```
```
