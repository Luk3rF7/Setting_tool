<h1 align="center"> Props types </h1>


<p>a gente precisa fazer uma validações das props </p>

<h3>iniciando props :</h3>

<li> npm i props-types </li>

             import  P from 'prop-types'
            export class Button extends Component {
  
                render(){
                  const { text, onClicks,disabled } = this.props
                  return (
                                 <button 
                    className='button'
                    onClick={onClicks}
                    disabled={disabled}
                    >
                      {text}
                      </button>
                  )
                }
              }

              aqui eu passo configuração padroes do elem
              Button.defaultProps = {
                disabled:false,
              }
                aqui passo os tipo que são as props: string,number,bool,func etc...
                e ja defino se e requirido ou não
              Button.propstypes = {
                text: P.string.isRequired,
                onClick: P.func.isRequired,
                disabled:P.bool
              }

<p>a gente utiliza props quando recebemos algo dentro de components </p>

<p>modo complexo com array </p>


          Post.propTypes = {
            post: P.arrayOf(P.shape({
              title: Props.string.isRequired,
              cover: Props.string.isRequired,
              body: Props.string.isRequired,
              id: Props.number.isRequired,
            })),
          }

<li>arrayOf e um array de</li>
<li>P.shape() e um objeto a forma de um objeto
ai dentro eu passo a forma que e meu posto</li>