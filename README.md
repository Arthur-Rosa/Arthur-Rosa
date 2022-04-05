```java
@Controller
public class ArthurController extends Developer {

	@Autowired
	private ArthurRepository repArthur;

	@RequestMapping("aboutYou")
	public String aboutMe(Model model) {
    		Arthur art =  new Arthur();
    
    		art.setName(" Arthur Rosa ");
    		art.setEmail(" arthur.corporativo@outlook.com ");
    		art.setLinkedin(" https://www.linkedin.com/in/arthur-rosa-a2805b208/ ");
  
  		model.addAttribute("arthur", art);
		return "arthur/about";
	}

	@RequestMapping("languages")
	public String languages(Model model) {
		
		List<String> lang = new ArrayList<String>();
    
    		lang.add(" JavaScript ");
    		lang.add(" Php ");
    		lang.add(" Java ");
    		lang.add(" Sql ");
    		lang.add(" SpringBoot ");
    		lang.add(" Hibernate ");
    
		model.addAttribute("languages", lang);
		return "arthur/languages";
	}

}
```
 <div style="display: inline_block" align="center"><br>
     <img align="center" alt="html" width="40px" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/html5/html5-original.svg" />
     <img align="center" alt="css" width="40px" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/css3/css3-original.svg" />
     <img align="center" alt="js" width="40px" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/javascript/javascript-original.svg" />
     <img align="center" alt="java" width="40px" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/java/java-original.svg" />
     <img align="center" alt="react" width="40px" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/react/react-original.svg" />
     <img align="center" alt="spring" width="40px" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/spring/spring-original-wordmark.svg" />
     <img align="center" alt="android-studio" width="40px" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/androidstudio/androidstudio-original.svg" />
     <img align="center" alt="vscode" width="40px" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/vscode/vscode-original.svg" />
   </div>
