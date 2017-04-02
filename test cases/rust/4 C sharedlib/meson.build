project('rust shared C library', ['rust', 'c'])

l = shared_library('stuff', 'stuff.rs',
  rust_args: ['--crate-type', 'cdylib'],
  install : true
)
e = executable('prog', 'prog.c', link_with : l, install : true)
test('linktest', e)
