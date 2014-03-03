package test1;

import org.eclipse.swt.SWT;
import org.eclipse.swt.graphics.Point;
import org.eclipse.swt.graphics.Rectangle;
import org.eclipse.swt.layout.FillLayout;
import org.eclipse.swt.layout.FormLayout;
import org.eclipse.swt.widgets.Button;
import org.eclipse.swt.widgets.Combo;
import org.eclipse.swt.widgets.Composite;
import org.eclipse.swt.widgets.Display;
import org.eclipse.swt.widgets.Label;
import org.eclipse.swt.widgets.Menu;
import org.eclipse.swt.widgets.MenuItem;
import org.eclipse.swt.widgets.Shell;
import org.eclipse.swt.widgets.Table;
import org.eclipse.swt.widgets.TableColumn;
import org.eclipse.swt.widgets.Text;

import com.cloudgarden.resource.SWTResourceManager;


/**
* This code was edited or generated using CloudGarden's Jigloo
* SWT/Swing GUI Builder, which is free for non-commercial
* use. If Jigloo is being used commercially (ie, by a corporation,
* company or business for any purpose whatever) then you
* should purchase a license for each developer using Jigloo.
* Please visit www.cloudgarden.com for details.
* Use of Jigloo implies acceptance of these licensing terms.
* A COMMERCIAL LICENSE HAS NOT BEEN PURCHASED FOR
* THIS MACHINE, SO JIGLOO OR THIS CODE CANNOT BE USED
* LEGALLY FOR ANY CORPORATE OR COMMERCIAL PURPOSE.
*/
public class test1 extends org.eclipse.swt.widgets.Composite {

	private Menu menu1;
	private MenuItem aboutMenuItem;
	private MenuItem contentsMenuItem;
	private Menu helpMenu;
	private MenuItem helpMenuItem;
	private TableColumn tableColumn1;
	private Button button2;
	private Button button1;
	private Text text3;
	private Label label3;
	private Text text2;
	private Label label2;
	private Text text1;
	private Label label1;
	private Composite composite1;
	private Button Rejectbutton;
	private Button Approvebutton;
	private TableColumn tableColumn5;
	private TableColumn tableColumn4;
	private TableColumn tableColumn3;
	private TableColumn tableColumn2;
	private Table purchasetable;
	private Combo userlistCombo;
	private MenuItem exitMenuItem;
	private MenuItem closeFileMenuItem;
	private MenuItem saveFileMenuItem;
	private MenuItem newFileMenuItem;
	private MenuItem openFileMenuItem;
	private Menu fileMenu;
	private MenuItem fileMenuItem;

	{
		//Register as a resource user - SWTResourceManager will
		//handle the obtaining and disposing of resources
		SWTResourceManager.registerResourceUser(this);
	}

	public test1(Composite parent, int style) {
		super(parent, style);
		initGUI();
	}
	
	/**
	* Initializes the GUI.
	*/
	private void initGUI() {
		try {
			this.setSize(742, 339);
			this.setBackground(SWTResourceManager.getColor(192, 192, 192));
			this.setLayout(null);
			{
				userlistCombo = new Combo(this, SWT.NONE);
				userlistCombo.setText("Users");
				userlistCombo.setSize(36, 37);
				userlistCombo.setBounds(50, 30, 60, 23);
			}
			{
				purchasetable = new Table(this, SWT.NONE);
				purchasetable.setBounds(50, 75, 303, 146);
				purchasetable.setLinesVisible(true);
				purchasetable.setHeaderVisible(true);
				{
					tableColumn1 = new TableColumn(purchasetable, SWT.NONE);
					tableColumn1.setText("Item");
					tableColumn1.setWidth(60);
				}
				{
					tableColumn2 = new TableColumn(purchasetable, SWT.NONE);
					tableColumn2.setText("Price");
					tableColumn2.setWidth(60);
				}
				{
					tableColumn3 = new TableColumn(purchasetable, SWT.NONE);
					tableColumn3.setText("Quantity");
					tableColumn3.setWidth(60);
				}
				{
					tableColumn4 = new TableColumn(purchasetable, SWT.NONE);
					tableColumn4.setText("Status");
					tableColumn4.setWidth(60);
				}
				{
					tableColumn5 = new TableColumn(purchasetable, SWT.NONE);
					tableColumn5.setText("ID");
					tableColumn5.setWidth(60);
				}
			}
			{
				Approvebutton = new Button(this, SWT.PUSH | SWT.CENTER);
				Approvebutton.setText("Approve");
				Approvebutton.setSize(60, 30);
				Approvebutton.setBounds(50, 246, 60, 30);
			}
			{
				Rejectbutton = new Button(this, SWT.PUSH | SWT.CENTER);
				Rejectbutton.setText("Reject");
				Rejectbutton.setSize(60, 30);
				Rejectbutton.setBounds(276, 246, 60, 30);
			}
			{
				composite1 = new Composite(this, SWT.NONE);
				composite1.setLayout(null);
				composite1.setBounds(375, 40, 335, 206);
				{
					label1 = new Label(composite1, SWT.NONE);
					label1.setText("Item :");
					label1.setBounds(33, 19, 39, 18);
				}
				{
					text1 = new Text(composite1, SWT.NONE);
					text1.setBounds(83, 13, 188, 30);
				}
				{
					label2 = new Label(composite1, SWT.NONE);
					label2.setText("Price");
					label2.setBounds(29, 67, 43, 18);
				}
				{
					text2 = new Text(composite1, SWT.NONE);
					text2.setBounds(83, 61, 188, 30);
				}
				{
					label3 = new Label(composite1, SWT.NONE);
					label3.setText("Quantity :");
					label3.setBounds(12, 110, 60, 16);
				}
				{
					text3 = new Text(composite1, SWT.NONE);
					text3.setBounds(83, 103, 187, 30);
				}
				{
					button1 = new Button(composite1, SWT.PUSH | SWT.CENTER);
					button1.setText("Add PO");
					button1.setSize(60, 30);
					button1.setBounds(168, 264, 60, 30);
				}
				{
					button2 = new Button(composite1, SWT.PUSH | SWT.CENTER);
					button2.setText("Add PO");
					button2.setBounds(210, 150, 60, 30);
				}
			}
			{
				menu1 = new Menu(getShell(), SWT.BAR);
				getShell().setMenuBar(menu1);
				{
					fileMenuItem = new MenuItem(menu1, SWT.CASCADE);
					fileMenuItem.setText("File");
					{
						fileMenu = new Menu(fileMenuItem);
						{
							openFileMenuItem = new MenuItem(fileMenu, SWT.CASCADE);
							openFileMenuItem.setText("Open");
						}
						{
							newFileMenuItem = new MenuItem(fileMenu, SWT.CASCADE);
							newFileMenuItem.setText("New");
						}
						{
							saveFileMenuItem = new MenuItem(fileMenu, SWT.CASCADE);
							saveFileMenuItem.setText("Save");
						}
						{
							closeFileMenuItem = new MenuItem(fileMenu, SWT.CASCADE);
							closeFileMenuItem.setText("Close");
						}
						{
							exitMenuItem = new MenuItem(fileMenu, SWT.CASCADE);
							exitMenuItem.setText("Exit");
						}
						fileMenuItem.setMenu(fileMenu);
					}
				}
				{
					helpMenuItem = new MenuItem(menu1, SWT.CASCADE);
					helpMenuItem.setText("Help");
					{
						helpMenu = new Menu(helpMenuItem);
						{
							contentsMenuItem = new MenuItem(helpMenu, SWT.CASCADE);
							contentsMenuItem.setText("Contents");
						}
						{
							aboutMenuItem = new MenuItem(helpMenu, SWT.CASCADE);
							aboutMenuItem.setText("About");
						}
						helpMenuItem.setMenu(helpMenu);
					}
				}
			}
			this.layout();
		} catch (Exception e) {
			e.printStackTrace();
		}
	}
	
	/**
	* Auto-generated main method to display this 
	* org.eclipse.swt.widgets.Composite inside a new Shell.
	*/
	public static void main(String[] args) {
		Display display = Display.getDefault();
		Shell shell = new Shell(display);
		test1 inst = new test1(shell, SWT.NULL);
		Point size = inst.getSize();
		shell.setLayout(new FillLayout());
		shell.layout();
		if(size.x == 0 && size.y == 0) {
			inst.pack();
			shell.pack();
		} else {
			Rectangle shellBounds = shell.computeTrim(0, 0, size.x, size.y);
			shell.setSize(shellBounds.width, shellBounds.height);
		}
		shell.open();
		while (!shell.isDisposed()) {
			if (!display.readAndDispatch())
				display.sleep();
		}
	}

}
