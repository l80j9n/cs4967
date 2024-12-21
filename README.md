java c
PROGRAMMING IT 
(COMPSCI 4039) 
Monday 12 December 2022Important note: throughout this exam, whenever you are asked to write Java code, do not worry about whether your code compiles.    The markers will never test any submitted code from this exam. 
1.          (a) The International Olympic committee are designing an   IT   system, built   in   Java,   that   will
record the medal tables in their summer and winter   games.   The following class will be used to represent a team:
public class 
Team { 
private 
String name; 
private 
int numGold; 
private int numSilver; 
private int numBronze; 
} 
Here, name is the team name (for instance, “Ireland”), and numGold,   numSilver,   and   numBronze are the total   numbers   of gold,   silver   and   bronze   medals   that   the   team   has   accumulated so far in the   competition.
(i)      Write a constructor for the Team class that   is   called   bypassing   only   the   team   name.   This should set name to be the passed   string   and   initialise   numGold,   numSilver   and numBronze to 0. [3] 
(ii)      Write a second constructor that takes four parameters to add   a team to   the   table   after 
they   have   already   been   awarded   medals.   The   four   parameters   should   be   the   team   name String as well as three integers for the numbers of medals already   won by   that   team.    [4]
(b) Create   getter   and   setter   methods   for   the   name   string   and   the   three   integer   attributes   (i.e.   the medal   counts) of   the   Team   class.    [8]
2.          (a) Since   each   team   can   only   win   at   most   1   medal   of   each   kind   for   any   given   event,   overload the   setter   methods   for   the   medal   counts   so   that   the   new   version   is   passed   no   parameters   and simply   increments   the   count   by   1. [3] 
(b) Create a method within the   Team class   that   will   allow   the   team   name   and   medal   counts for each team to be printed out using a   System   .out   .println(t), where tis a Team   object.   The   team   name, number   of   golds, number   of   silver   and   number   of   bronze   should   be printed out in that order, in the fixed width order   given   below   (note   that   the   periods   should   be printed as spaces – periods are   just being used in this   diagram   so   you   can   count   them   easily):
Australia   .   .   .   .   .   . |   .   .   .   17   |   .   .   .   .7   |   .   .   .22                                                                            [7]
(c) A   class   in   now   required   to   hold   the   leaderboard   for   the   games,   in   an   array   of   Team   objects.   Part   of   this   class   is   as   follows:public      class      Leaderboard      {private    int    numTeams;private      Team[]      teams;
}Write a constructor for this leaderboard class.   The constructor should take a single   parameter, an   integer   representing   the   number   of   Teams   competing   at   the   games.   The   number   of   teams should be   stored in   numTeams and this value   should   be   used   to   instantiate   teams,   the   array   of   Team   objects.       [3]
(d) Give   the   command   that   could   have   been   used   to   initialise   a   leaderboard   for   this   year’s   Beijing   Winter   Olympics, in   which   91 teams   took   part.       [2]
3.          (a) The   code   shown   below   is   an   attempt   by   the   college   in   printing   a   simple   welcoming   message for the new   students   of this   semester.    Unfortunately, the code will   not   work.    Identify 4   mistakes   that   can   be   found   in   the   code.
public    class    Welcome    New    Students    {
static      void      main(String[]     代 写COMPSCI 4039 PROGRAMMING IT 2022Java
代做程序编程语言 args)      {
System   .out   .println(Welcome    students!)
}
}                                                                                                                                                                                                        [4]
(b) The   college   is   asking   developers   to   find   a   way   of   sorting   out   the   student’s   records.
(i)    In   the   first   part   the   developers   need   to   identify   the   highest   grade.
You   are   asked   to   create   a   methods   that   can   be   used   to   identify   and   print   out   the   highest grade.
Assume that the marks are in an integer format and the records   are   saved   as   an   array.   For   the   array   use   the   values   25,   89,   95,   60, 45,78. [7] 
(ii)      Write another function in the same class you created for   Q3bi in   order   to   identify   the 
lowest grade.   The lowest grade should also be printed.   All the details   are the   same   as   presented   in   3bi.       [4]
4.          (a) One   student’s   surname   was   entered   wrongly   in   the   students’   text   record.   His   surname   was “Ferguson” but   the   entry   was “Farguson”   .(i)      Write   a   method   that   can   easily   check   if   the   wrongly   typed   student’s   surname   is   in   the 		text file.   This means that the method should return true if the line is found or false if   		it   is   not.   Assume   that   the   path   of   the   file   is   just “filepath”, the   name   of   the   text   file   is 	“Srecord” and no newline   characters are included.   Error handling for   FileNotFound   			should   be   considered.                                                                                        [4](ii)    After   producing   code   for   reading   the   text   file   (4ai) include   additional   code   that   should be included in the previous method, for replacing the wrong surname   (Farguson) with the correct one (Ferguson).   Make sure to include a printout   of the updated   surname.         [2] 
(iii)      What would be the difference if we wanted to replace any entries having the   surname   “Farguson”   with   an   empty   line?    Write   how   the   previous   code   from   4aii   would   be   modified so the entry ”Farguson” would be replaced with an empty   line   instead.
Write   the   relevant   code.                                                                                                                                                                                                                                                                                           [1]
(b) For   the   same   course   a   string   array   was   created   called   “Sname”   which   produces   as   an   output the names   of the   students in   an   alphabetical   order.    The following names were   included   (Thomas,Amaya, Gustavo, Melina, Reirse, Bell).   This is a bad coding example and there   are several mistakes in the code.   You are asked to   identify   8   mistakes   and point   them   out,   explaining them.
Class      AlphName{
public      static      void      main{   int      n      =      0;
String    Sname[]    =    {"Thomas,    Amaya,    Gustavo,   Melina,      Reirse,      Bell"};
String      temp
for         (int      i      =      0;      i      < n;) {
for         (    k    =    100;    k    < n; k++) {
if         (Sname[i]   .compareTo(Sname[k])      >0{   temp    =    Sname[i];
Sname[i]    =    Sname[k];   Sname[k]    =    temp;
}   }
}
System   .println("Names      in      alphabetical      order:");   for         (int      i      =      0;      i      < n; i++) {
System   .out   .println();   }
}   }[8]





         
加QQ：99515681  WX：codinghelp  Email: 99515681@qq.com
