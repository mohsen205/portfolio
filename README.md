```
import React from 'react'
import style from '../../styles/utils/progressBar.module.css'
const ProgressBar = ({ progressPercentage , ultimateGoad}) => {
    return (
        <div className={`${style.progress} d-flex  pt-2`}>
            <div className='col-2'>
                <p>{progressPercentage} % ETH LOCKED</p>
            </div>
            <div className='col-8'>
                <div className={`${style.progressCore} progress`}>
                    <div className={`${style.bar} progress-bar`} role="progressbar" style={{ width: `${progressPercentage}%` }} aria-valuenow={progressPercentage} aria-valuemin="0" aria-valuemax="100"></div>
                </div>
            </div>
            <div className='col-2'>
                <p> {ultimateGoad} ETH GOAL</p>
            </div>
        </div>
    )         
}

export default ProgressBar

```
