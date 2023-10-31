# React js dynamic table column show hide 

```javascript

import { useEffect, useRef, useState } from "react";

const Datatable = ()=>{
    const [headerMap, setHeaderMap] = useState([
        {
            label:'Checkbox',
            id:'_checkbox',
            show:true,
        },
        {
            label:'User',
            id:'_user',
            show:true,
        },
        {
            label:'Email',
            id:'_email',
            show:true,
        },
        {
            label:'Phone',
            id:'_phone',
            show:true,
        },
    ])
    
    const toggle = (item, index)=>{
        item.show = !item.show
        setHeaderMap((prev)=>{
            var temp = [...prev];
            temp.splice(index, 1, item)
            return temp;
        })
    }



    return (
        <>
                <ul>
                    {
                        headerMap.map((item, index)=>(
                            <li key={index+1}>
                                <label>
                                    <input
                                    defaultChecked={item.show}
                                    onChange={()=>toggle(item, index)} 
                                    className="me-2"  
                                    type="checkbox" />
                                    { item.label }
                                </label>
                            </li>
                        ))
                    }
                </ul>
                <table className="table table-sm table-bordered">
                    <thead>
                        <tr>
                            {headerMap[0].show && <td><input type="checkbox" /></td> }
                            {headerMap[1].show && <td>User</td> }
                            {headerMap[2].show && <td>Email</td> }
                            {headerMap[3].show && <td>Phone</td> }
                        </tr>
                    </thead>
                    <tbody>
                        <tr>
                            {headerMap[0].show && <td><input type="checkbox" /></td>}
                            {headerMap[1].show && <td><img style={{ borderRadius:'50%' }} src={`${'https://i.pravatar.cc/50?'}${Math.random()}`} width={30} alt="" /></td>}
                            {headerMap[2].show && <td>example@gmail.com</td> }
                            {headerMap[3].show && <td>+88 0123456789</td> }
                        </tr>
                        <tr>
                            {headerMap[0].show && <td><input type="checkbox" /></td>}
                            {headerMap[1].show && <td><img style={{ borderRadius:'50%' }} src={`${'https://i.pravatar.cc/50?'}${Math.random()}`} width={30} alt="" /></td>}
                            {headerMap[2].show && <td>example@gmail.com</td> }
                            {headerMap[3].show && <td>+88 0123456789</td> }
                        </tr>
                        <tr>
                            {headerMap[0].show && <td><input type="checkbox" /></td>}
                            {headerMap[1].show && <td><img style={{ borderRadius:'50%' }} src={`${'https://i.pravatar.cc/50?'}${Math.random()}`} width={30} alt="" /></td>}
                            {headerMap[2].show && <td>example@gmail.com</td> }
                            {headerMap[3].show && <td>+88 0123456789</td> }
                        </tr>
                        <tr>
                            {headerMap[0].show && <td><input type="checkbox" /></td>}
                            {headerMap[1].show && <td><img style={{ borderRadius:'50%' }} src={`${'https://i.pravatar.cc/50?'}${Math.random()}`} width={30} alt="" /></td>}
                            {headerMap[2].show && <td>example@gmail.com</td> }
                            {headerMap[3].show && <td>+88 0123456789</td> }
                        </tr>
                        <tr>
                            {headerMap[0].show && <td><input type="checkbox" /></td>}
                            {headerMap[1].show && <td><img style={{ borderRadius:'50%' }} src={`${'https://i.pravatar.cc/50?'}${Math.random()}`} width={30} alt="" /></td>}
                            {headerMap[2].show && <td>example@gmail.com</td> }
                            {headerMap[3].show && <td>+88 0123456789</td> }
                        </tr>
                        <tr>
                            {headerMap[0].show && <td><input type="checkbox" /></td>}
                            {headerMap[1].show && <td><img style={{ borderRadius:'50%' }} src={`${'https://i.pravatar.cc/50?'}${Math.random()}`} width={30} alt="" /></td>}
                            {headerMap[2].show && <td>example@gmail.com</td> }
                            {headerMap[3].show && <td>+88 0123456789</td> }
                        </tr>
                        <tr>
                            {headerMap[0].show && <td><input type="checkbox" /></td>}
                            {headerMap[1].show && <td><img style={{ borderRadius:'50%' }} src={`${'https://i.pravatar.cc/50?'}${Math.random()}`} width={30} alt="" /></td>}
                            {headerMap[2].show && <td>example@gmail.com</td> }
                            {headerMap[3].show && <td>+88 0123456789</td> }
                        </tr>
                        <tr>
                            {headerMap[0].show && <td><input type="checkbox" /></td>}
                            {headerMap[1].show && <td><img style={{ borderRadius:'50%' }} src={`${'https://i.pravatar.cc/50?'}${Math.random()}`} width={30} alt="" /></td>}
                            {headerMap[2].show && <td>example@gmail.com</td> }
                            {headerMap[3].show && <td>+88 0123456789</td> }
                        </tr>
                        <tr>
                            {headerMap[0].show && <td><input type="checkbox" /></td>}
                            {headerMap[1].show && <td><img style={{ borderRadius:'50%' }} src={`${'https://i.pravatar.cc/50?'}${Math.random()}`} width={30} alt="" /></td>}
                            {headerMap[2].show && <td>example@gmail.com</td> }
                            {headerMap[3].show && <td>+88 0123456789</td> }
                        </tr>
                        <tr>
                            {headerMap[0].show && <td><input type="checkbox" /></td>}
                            {headerMap[1].show && <td><img style={{ borderRadius:'50%' }} src={`${'https://i.pravatar.cc/50?'}${Math.random()}`} width={30} alt="" /></td>}
                            {headerMap[2].show && <td>example@gmail.com</td> }
                            {headerMap[3].show && <td>+88 0123456789</td> }
                        </tr>
                        <tr>
                            {headerMap[0].show && <td><input type="checkbox" /></td>}
                            {headerMap[1].show && <td><img style={{ borderRadius:'50%' }} src={`${'https://i.pravatar.cc/50?'}${Math.random()}`} width={30} alt="" /></td>}
                            {headerMap[2].show && <td>example@gmail.com</td> }
                            {headerMap[3].show && <td>+88 0123456789</td> }
                        </tr>
                        <tr>
                            {headerMap[0].show && <td><input type="checkbox" /></td>}
                            {headerMap[1].show && <td><img style={{ borderRadius:'50%' }} src={`${'https://i.pravatar.cc/50?'}${Math.random()}`} width={30} alt="" /></td>}
                            {headerMap[2].show && <td>example@gmail.com</td> }
                            {headerMap[3].show && <td>+88 0123456789</td> }
                        </tr>
                        <tr>
                            {headerMap[0].show && <td><input type="checkbox" /></td>}
                            {headerMap[1].show && <td><img style={{ borderRadius:'50%' }} src={`${'https://i.pravatar.cc/50?'}${Math.random()}`} width={30} alt="" /></td>}
                            {headerMap[2].show && <td>example@gmail.com</td> }
                            {headerMap[3].show && <td>+88 0123456789</td> }
                        </tr>
                        <tr>
                            {headerMap[0].show && <td><input type="checkbox" /></td>}
                            {headerMap[1].show && <td><img style={{ borderRadius:'50%' }} src={`${'https://i.pravatar.cc/50?'}${Math.random()}`} width={30} alt="" /></td>}
                            {headerMap[2].show && <td>example@gmail.com</td> }
                            {headerMap[3].show && <td>+88 0123456789</td> }
                        </tr>
                    </tbody>
                </table>
        </>
    );
}

export default Datatable;



```

## Output

![alt text](https://github.com/sourovpal/react-js-dynamic-table-column-show-hide/blob/master/screenshot_1.png?raw=true)
