# copy permission

here only talk about the command like
```bash
copy src_dir/src_file tgt_dir/tgt_file
```

check the copy workflow

1. check file exist? y -> 3, n -> 2
2. create a new file in the directory.
3. write the content into the file.

On step 2, the operation require the write permission of the target directoy.
On step 3, the operation require the write permission of the target file.

For these requirements, there are 2 intereting cases.

1. the target file doesn't exist, we need the write permission of the target directory to create new file.
2. the target file exist, we only need the write permission of the target file to overwrite.
