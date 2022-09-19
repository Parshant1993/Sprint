# Sprint for automate firs Seleniumprogramme
test
package com.Selenum;



import org.openqa.selenium.Dimension;
import org.openqa.selenium.Point;
import org.openqa.selenium.WebDriver;
import org.openqa.selenium.chrome.ChromeDriver;

public class InvokeBowwse {

	public static void main(String[] args) throws InterruptedException {
		// TODO Auto-generated method stub
		System.setProperty("webdriver.chrome.driver","D:\\Tools\\ChromeDriver\\chromedriver.exe");
	                   // key and path in laptop
	 ChromeDriver driver = new ChromeDriver();
	 
		//driver.navigate().to("https://www.google.co.in/");
	
	Thread.sleep(4000);
	 driver.navigate().back();
	 Thread.sleep(4000);
	 driver.navigate().refresh();
	 Thread.sleep(4000);
	 driver.navigate().forward();
	 Thread.sleep(4000);

	driver.manage().window().maximize();// to maximise winow 
    driver.get("https://github.com/search?q=compile+with+problem");
    String pagetitle = driver.getTitle();
    System.out.println(pagetitle);
  //  System.out.println(driver.getTitle());
    System.out.println(driver.getCurrentUrl());
   
    driver.close();
   // set the size of brower
	 Thread.sleep(9000);

    Dimension d = new Dimension(600,900);
    driver.manage().window().setSize(d);
    Thread.sleep(7000);
Point p= new Point(100,100);
Thread.sleep(7000);
driver.manage().window().setPosition(p);
Thread.sleep(9000);
  //  driver.quit();
    
