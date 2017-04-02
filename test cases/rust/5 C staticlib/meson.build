project('rust static C library', ['rust', 'c'])

l = static_library('stuff', 'stuff.rs',
  rust_args: ['--crate-type', 'staticlib']
)
e = executable('prog', 'prog.c', link_with : l, install : true)
test('linktest', e)
