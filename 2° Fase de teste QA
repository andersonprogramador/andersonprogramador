import org.junit.jupiter.api.Test;
import org.openqa.selenium.By;
import org.openqa.selenium.WebDriver;
import org.openqa.selenium.chrome.ChromeDriver;

public class SwagLabs {

    @Test
    public void suagLabs() throws InterruptedException {
        // Instância do driver
        System.setProperty("webdriver.chrome.driver", "/home/guilherme/App's/Driver/chromedriver");
        WebDriver driver = new ChromeDriver();

        //Acesso ao site
        driver.navigate().to("https://www.saucedemo.com/");


        //Login
        driver.findElement(By.id("user-name")).sendKeys("standard_user");
        driver.findElement(By.id("password")).sendKeys("secret_sauce");
        driver.findElement(By.id("login-button")).click();

        //Filtro
        driver.findElement(By.xpath("//select")).click();
        driver.findElement(By.xpath("//option[@value='lohi']")).click();

        //Adicionar compras ao carrinho
        driver.findElement(By.xpath("//img[@alt='Sauce Labs Onesie']")).click();
        driver.findElement(By.id("add-to-cart-sauce-labs-onesie")).click();
        driver.findElement(By.id("back-to-products")).click();

        driver.findElement(By.xpath("//img[@alt='Test.allTheThings() T-Shirt (Red)']")).click();
        driver.findElement(By.id("add-to-cart-test.allthethings()-t-shirt-(red)")).click();

        //Checkout
        driver.findElement(By.xpath("//div[@id='shopping_cart_container']/a")).click();
        driver.findElement(By.id("checkout")).click();
        driver.findElement(By.id("first-name")).sendKeys("José");
        driver.findElement(By.id("last-name")).sendKeys("Silva");
        driver.findElement(By.id("postal-code")).sendKeys("04916000");

        driver.findElement(By.id("continue")).click();
        driver.wait(5);

        //Finalizar comprar
        driver.findElement(By.id("finish")).click();

        //Fechar o driver.
        driver.quit();
    }
}
