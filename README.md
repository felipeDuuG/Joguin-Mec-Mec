# Joguin-Mec-Mec
meu bonde

Program Pzim ;
var
resp:integer;
campo:array[1..3,1..3] of string;
jogada:integer;
cont_jogador:integer;
jogada_ok:boolean;
jogador:array [1..2] of string;
l,c:integer;
//PROCEDIMENTO MENU
procedure menu();
var
i:integer;
begin
  gotoxy(19,3);
  writeln('     __                 ____ _   __    ____');
  gotoxy(19,4);
  writeln(' __ / /__  ___ ____  __/ / /| | / /__ / / /  ___ _');
  gotoxy(19,5);
  writeln('/ // / _ \/ _ `/ _ \/_  . __/ |/ / -_) / _ \/ _ `/');
  gotoxy(19,6);
  writeln('\___/\___/\_, /\___/_    __/|___/\__/_/_//_/\_,_/');
  gotoxy(19,7);
  writeln('         /___/      /_/_/                        ');
  
  gotoxy(23,9);
  writeln('***************************************');
  gotoxy(23,10);
  writeln('*            1-Iniciar Jogo           *');
  gotoxy(23,11);
  writeln('*            2-Desenvolvedores        *');
  gotoxy(23,12);
  writeln('***************************************');
  gotoxy(25,13);
  write('Escolha uma opção: ');
  readln(resp); 
  clrscr;
  
end;


 //PROGRAMA PRINCIPAL
 
Begin
  menu();
  if (resp = 1) then
  begin
    for l:= 1 to 3 do
    begin
      for c:= 1 to 3 do
      begin
        campo[l,c] := ' ';
      end;
    end;
    
 
for cont_jogador:= 1 to 2 do
begin
 gotoxy (35,3);
writeln ('JOGADORES');
gotoxy (25,5);
write ('Digite o nome do JOGADOR ',cont_jogador,': ');
read(jogador[cont_jogador]);
clrscr;
end;
cont_jogador:=1;





//Exibe instruções    
gotoxy(35,3);    
writeln('INSTRUÇÕES');
gotoxy (15,5);
writeln ('O Jogador 1 começa, digite o numero de 1 a 9 usando');
gotoxy (15,6);
writeln ('o teclado numerico correspondente as ''casas'', quem');
gotoxy (15,7);
writeln ('completar uma linha vertical horizontal ou diagonal');
gotoxy (15,9);
writeln ('PRESSIONE QUALQUER TECLA PARA COMEÇAR...');
readkey;
clrscr; // Limpa a tela


//Desenha o jogo da velha
            
      writeln;
       gotoxy(30,5); 
      writeln('  ', campo[1, 1], ' | ', campo[1, 2], ' | ', campo[1, 3]);
       gotoxy(30,6); 
      writeln(' -----------');
       gotoxy(30,7); 
      writeln('  ', campo[2, 1], ' | ', campo[2, 2], ' | ', campo[2, 3]);
       gotoxy(30,8); 
      writeln(' -----------');
       gotoxy(30,9); 
      writeln('  ', campo[3, 1], ' | ', campo[3, 2], ' | ', campo[3, 3]);
      writeln;
      
  write('Vez do JOGADOR 1:');
  read(jogada;
			      
end;
  
End.
