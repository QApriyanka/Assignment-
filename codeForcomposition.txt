package Steps;

import java.util.concurrent.TimeUnit;
import org.openqa.selenium.By;
import org.openqa.selenium.WebDriver;
import org.openqa.selenium.WebElement;
import org.openqa.selenium.chrome.ChromeDriver;
import org.openqa.selenium.support.ui.ExpectedConditions;
import org.openqa.selenium.support.ui.WebDriverWait;

import io.cucumber.java.en.Given;
import io.cucumber.java.en.Then;
import io.cucumber.java.en.When;

public class Step1 {
	
	WebDriver driver = null;
	
	@Given("user is on login page")
	public void user_is_on_login_page() {
		
		
	System.setProperty("webdriver.chrome.driver","C:\\Users\\admin\\Desktop\\lagan\\chromedriver_win32 (1)");
	 driver = new ChromeDriver();
	driver.get("https://gmail.com/");
	  driver.manage().window().maximize();
	  driver.findElement(By.linkText("Sign in")).click();
	  
	    throw new io.cucumber.java.PendingException();
	    
	}

	@When("user enters jok49729@gmail.com and Okay@{int}")
	public void user_enters_jok49729_gmail_com_and_okay(Integer int1) throws InterruptedException{
		
		driver.findElement(By.xpath("//*[@id='identifierId']")).sendKeys("jok49729_gmail_com");
		driver.findElement(By.xpath("//*[@id=\'identifierNext\']/div/button")).click();
		driver.findElement(By.xpath("//*[@id='password']")).sendKeys("xyz@123");
		
		Thread.sleep(2000);
	   
	    throw new io.cucumber.java.PendingException();
	}

	@When("clicks next button")
	public void clicks_next_button() {
		
		driver.findElement(By.xpath("//*[@id=\'passwordNext\']/div/button/div[2]")).click();
	    
		// Write code here that turns the phrase above into concrete actions
	    throw new io.cucumber.java.PendingException();
	}

	@Then("user is navigated to mail Inbox page")
	public void user_is_navigated_to_mail_inbox_page() {
	    // Write code here that turns the phrase above into concrete actions
	    throw new io.cucumber.java.PendingException();
	}

	@Given("user has successfully logged into gmail account")
	public void user_has_successfully_logged_into_gmail_account() {
	    // Write code here that turns the phrase above into concrete actions
	    throw new io.cucumber.java.PendingException();
	}

	@Given("user clicks on composition button")
	public void user_clicks_on_composition_button() {
	   
		driver.findElement(By.cssSelector("#\\:34 > div > div")).click();
		
		// Write code here that turns the phrase above into concrete actions
	    throw new io.cucumber.java.PendingException();
	}

	@Then("New window pops up with header New Message")
	public void new_window_pops_up_with_header_new_message() {
		
		
	    // Write code here that turns the phrase above into concrete actions
	    throw new io.cucumber.java.PendingException();
	}

	

}
