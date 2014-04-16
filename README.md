chess960-opening-book
=====================

Chess960 opening book in pgn format, depth 3, with 128137 unique starting positions and encoded castling.

I don't know about other software, but you can use it with cutechess-cli, providing the switch "variant". Here is an example:

`./cutechess-cli -variant fischerandom -rounds 100 -concurrency 2 -tournament gauntlet -pgnout SFvsSF100g_chess960.pgn -draw movenumber=40 movecount=10 score=10 -openings file=chess960_book_3moves.pgn format=pgn order=random plies=6 -engine name=stockfish cmd=stockfish -engine name=stockfish cmd=stockfish -each proto=uci option.Threads=1 option.OwnBook=false option.Hash=256 tc=60+0.5 timemargin=1000 whitepov`
