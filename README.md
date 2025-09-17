# Excel-sheet


=LET(
  txt, A2,
  pos, SEARCH("PRODUCT DESCRIPTION", txt),
  core, MID(txt, pos, LEN(txt)-pos+1),
  norm, TRIM(SUBSTITUTE(SUBSTITUTE(core, CHAR(10), " "), CHAR(13), " ")),
  s1, SUBSTITUTE(norm, " Size:", CHAR(10)&"Size:"),
  s2, SUBSTITUTE(s1, " Made In:", CHAR(10)&"Made In:"),
  s3, SUBSTITUTE(s2, " Color:", CHAR(10)&"Color:"),
  s3
)

