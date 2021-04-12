project('C# MONO_PATH', 'cs')

subdir('subdir1')
subdir('subdir2')

e = executable('prog', 'prog.cs', link_with : libb)

custom_target('cs_custom', output : 'output', command : [e, '@OUTPUT@'], build_by_default : true)

test('libtest', e)
