unit Unit1;

{$mode objfpc}{$H+}

interface

uses
  Classes, SysUtils, FileUtil, Forms, Controls, Graphics, Dialogs, StdCtrls,
  Grids;

type

  { TfrmSchleifen }

  TfrmSchleifen = class(TForm)
    btnRun: TButton;
    btn1mal1: TButton;
    grd1: TStringGrid;
    procedure btn1mal1Click(Sender: TObject);
    procedure btnRunClick(Sender: TObject);
  private
    { private declarations }
  public
    { public declarations }
  end;

var
  frmSchleifen: TfrmSchleifen;

implementation

{$R *.lfm}

{ TfrmSchleifen }

procedure TfrmSchleifen.btnRunClick(Sender: TObject);
var i : integer;
  c : Char;
begin
  for i:=2 to 6 do ShowMessage(IntToStr(i));
  for i:=5 downto 1 do ShowMessage(IntToStr(i));
  for c:='z' downto 'u' do ShowMessage(c);
end;

procedure TfrmSchleifen.btn1mal1Click(Sender: TObject);
var x, y : integer;
begin
  y:=1;  //initiale Werte setzen
  x:=1;
  while y < 11 do // Zeilen von 1..10 laufen lassen
        begin
             while x < 11 do // Spalten von 1..10 laufen lassen
               begin
                    grd1.Cells[x-1, y-1]:= IntToStr(x*y); //Zelle mit Produkt füllen
                    x:=x+1; //nächste Spalte
               end;
               y:=y+1; //nächste Zeile
               x:=1; // Spalte zurücksetzen auf Anfang
        end;

//for y:=1 to 10 do
//for x:=1 to 10 do
end;

end.

