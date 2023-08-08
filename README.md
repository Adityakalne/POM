# POM
My_POM
import org.openqa.selenium.By;
import org.openqa.selenium.WebDriver;
import org.openqa.selenium.WebElement;

public class UserPage {
    private WebDriver driver;

    public UserPage(WebDriver driver) {
        this.driver = driver;
    }

    // Locators
    private By chatWithMeButton = By.id("chat-button");
    private By previewImage1 = By.xpath("//img[@alt='Preview Image 1']");
    private By previewImage2 = By.xpath("//img[@alt='Preview Image 2']");
    private By unlockImageButton = By.id("unlock-button");

    // Methods
    public void clickChatWithMeButton() {
        driver.findElement(chatWithMeButton).click();
    }

    public void clickPreviewImage1() {
        driver.findElement(previewImage1).click();
    }

    public void clickPreviewImage2() {
        driver.findElement(previewImage2).click();
    }

    public void clickUnlockImageButton() {
        driver.findElement(unlockImageButton).click();
    }
}

