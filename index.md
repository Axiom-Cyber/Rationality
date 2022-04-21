# Rationality

Steps for solving easy CTF problems when you don't know anything about hacking.

## Assessing a Challenge

- [ ] Search up any terms you're unfamiliar with
- [ ] Check for any odd-sounding or weirdly-formatted words and Google them to check if they're hints
- [ ] Also note weird words as possible passwords which some programs require

## Determine Challenge Type

### I Have a Website URL

See page on [web exploitation](info/web.md)

### I Have a File

| Extension | Instructions |
| --- | --- |
| None | Run the `file` command to determine file type (`file path/to/file`). See next table for further instructions. |
| png, jpg, wav, mp3, mp4, pdf, docx | See page on [steganography](info/steganography.md). |
| txt | This could be encrypted text or a word list for bruteforcing |
| zip, 7z, tar, gz | This is a file archive. This is often done to save internet usage for transferring large files. See page on [decompression](info/decompression.md) then return back here when you've decompressed the file. |

| Return file type | Instructions |
| --- | --- |
| data/bytes | This is returned when even the file command has no idea what file you're dealing with |
| ELF Linux Binary | This is a Linux Binary. If it's under a category like buffer exploitation or pwning, see page on [binary exploitation](info/binary-exploitation.md). If it's under a category like reversing or forensics,, see page on [reverse engineering](reversing.md) |

### I Have an IP, Port, Extension-less File, and/or C Program

See page on [binary exploitation](info/binary-exploitation.md)

### I Have Some Encrypted Text

### I Don't Have Any of the Above
