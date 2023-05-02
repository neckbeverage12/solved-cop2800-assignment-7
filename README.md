Download Link: https://assignmentchef.com/product/solved-cop2800-assignment-7
<br>
Back to the gridiron.  Dolphins’ fans that have to work during the game are obsessed with staying connected to their team.  So, they register for real time alerts from an app that caters to their cravings.

Examine this driver:

public static void main (String [] arg) {

DolphinsFan john = new DolphinsFan (“john”);

DolphinsFan mike = new DolphinsFan (“mike”);

DolphinsFan ray = new DolphinsFan (“ray”);

DolphinsFan alice = new DolphinsFan (“alice”);

JetsFan steve = new JetsFan (“steve”);




SportsAlertsApp app = new SportsAlertsApp ();

app.registerForAlerts (john);

app.registerForAlerts (mike);

app.registerForAlerts (ray);

app.registerForAlerts (alice);

app.registerForAlerts (steve);




Scanner in = new Scanner (System.in);

for (int i=0;i&lt;5; i++) {

System.out.print (“

Who scored? (d or j)” );

if (in.next().equals(“d”))

app.sendOutAlert (Team.DOLPHINS);

else

app.sendOutAlert (Team.JETS);

}

}

<ul>

 <li>Class DolphinsFan and Class JetsFan extend an abstract class called SportsFan that has an abstract method reactToSportsAlert (Team t).</li>

 <li>Team is an enum.</li>

 <li>Class SportsAlertsApp aggregates SportsFan and sends out alerts to everyone when a team scores, polymorphically.</li>

</ul>




This is not a long program; your instructor’s was less than 75 lines including the driver.  If you find yourself writing a lot of code, ask for help.  Sample output on next page; output other than the prompt is from method reactToSportsAlert.  You can use this driver; I recommend that you do.




Please title your java file Assignment7.java.  Submitted files that do not compile will receive a grade of 0.