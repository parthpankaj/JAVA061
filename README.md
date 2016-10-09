# JAVA061
	import java.util.Calendar;
	import java.util.Timer;
	import java.util.TimerTask;

	public class TimerWithInitialDelay {
	public static void main(String args[]){
	         Timer timer = new Timer();
	         int initialDelay=5;
	         int consecutiveDelays=2;
	         final Calendar cal=Calendar.getInstance();
	         System.out.println("SimpleCodeStuffs!!! START "+cal.getTime()+"\n");
	         
	     timer.schedule(new TimerTask() {
	          public void run() {
	                  Calendar currentTime=Calendar.getInstance();
	                  System.out.println("SimpleCodeStuffs!!! TASK   "+currentTime.getTime());
	              }
	          }, (initialDelay*1000), consecutiveDelays * 1000);
	}
	}


***OUTPUT***
SimpleCodeStuffs!!! START Sun Oct 09 22:16:32 IST 2016
SimpleCodeStuffs!!! TASK   Sun Oct 09 22:16:37 IST 2016

