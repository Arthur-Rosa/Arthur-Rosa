```java
@Controller
public class ArthurController extends Developer {

	@Autowired
	private ArthurRepository repArthur;

	@RequestMapping("aboutYou")
	public String aboutMe() {
    		Arthur art =  new Arthur();
    
    		art.setName(" Arthur Rosa ");
    		art.setEmail(" arthur.corporativo@outlook.com ");
    		art.setLinkedin(" https://www.linkedin.com/in/arthur-rosa-a2805b208/ ");
  
		return "arthur/about";
	}

	@RequestMapping("languages")
	public String languages(Model model) {
		
		List<String> lang = new ArrayList<Integer>();
    
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
